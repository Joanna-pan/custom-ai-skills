# OpenClaw WebChat Delivery

Use this contract when delivering infographic files to an OpenClaw WebChat or Control UI session.

## Native Reply Attachments

For an ordinary WebChat final answer, attach each deliverable with an OpenClaw reply directive on its own plain-text line:

```text
MEDIA:/absolute/path/to/file.png
MEDIA:/absolute/path/to/file.pptx
MEDIA:/absolute/path/to/file.psd
```

The actual reply must not wrap these lines in a Markdown code fence. A directive must begin the line, use an absolute path or supported URL, and contain no prose on that line. Put explanatory text before or after the directive lines.

Before replying:

1. Confirm that every promised file exists, is readable, has the expected size, and is inside an OpenClaw-accessible workspace or media root.
2. Emit one `MEDIA:` line per file.
3. Do not replace a requested attachment with a Markdown link to `127.0.0.1`, `localhost`, or `file://`.

When the active source explicitly requires message-tool delivery, use `message(action="send")` with `media` for one file or `attachments: [{media: ...}]` for several files instead of `MEDIA:`. Follow the source session's output directives; do not use both mechanisms for the same attachment.

## What Does Not Count As Delivery

- Reading an image with `read` verifies or previews it for the model; an `inputImage` inside a tool result is not a durable reply attachment.
- Forwarding a tool result through a code-mode `image(...)` helper still leaves it in `custom_tool_call_output`; it does not guarantee that WebChat history will contain an attachment.
- A successful `curl` request proves that a temporary server can read the file, not that the user received it in chat.
- Do not claim that an image was attached until the final reply uses the native attachment path.

## Temporary Processes And Portals

Do not start a local HTTP server or Portal merely to deliver a static PNG, PPTX, or PSD. Use native reply attachments first.

If an interactive preview genuinely requires a server:

1. Track the returned process session and PID.
2. State whether the preview is temporary and how it is reached through the Control UI.
3. Stop and remove the background process before the final answer unless the user explicitly requested a persistent preview.
4. Confirm that the task ledger shows no active task left by the preview process.

Never leave a background server running as an attachment workaround; it can keep the Control UI task indicator active after the agent turn has completed.
