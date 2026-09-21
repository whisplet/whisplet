# Whisplet beta guide

This is the guide for the private beta. Read it before you install.

## What the beta is

Whisplet is a meeting copilot for Windows. It runs entirely on your own machine: speech
recognition, speaker labels and notes are all computed locally. The beta is a free, unsigned
build handed to a small number of known testers.

## What the beta is not

- It is not a finished product. It can crash, lose a recording, or mis-transcribe.
- It is not a supported release with guaranteed response times.
- It is not a cloud service. There is no account and no server-side copy of your meetings.
- It does not send your recordings or transcripts anywhere, ever.

## System requirements

- Windows 11.
- A microphone, and a way to capture system audio (the audio played by your own machine,
  for example the other side of a call).
- One of these hardware tiers:
  - CPU only
  - NVIDIA GPU
  - Intel Arc or Intel iGPU
  - AMD GPU
- Free disk space for the models included in the zip, about 7 GB, plus room for your own
  recordings and notes. [to confirm: minimum total free disk space recommended]

## Install

1. Download the beta zip from the link the maker sent you.
2. Unzip it to a folder of your choice. The zip contains a folder with the application and
   the models already inside; nothing else needs to be downloaded to start.
3. The beta is not signed, so Windows will warn you before the first launch. When you run the
   launcher, Windows shows a screen titled "Windows protected your PC". Click "More info",
   then click "Run anyway".
4. Windows Defender may take a moment to scan the folder the first time you run it. This is
   normal for an unsigned build; let it finish.
5. On first launch: [to confirm: what the app shows or asks for on its first run].

If Windows Defender flags the application as a threat rather than just warning about the
unknown publisher, tell the maker; see "How to report a bug" below.

## Daily use

This is an outline. Exact menu names, buttons and hotkeys are not final in the beta and will
be filled in.

1. Start Whisplet. [to confirm: how you start it, for example a shortcut or the launcher file]
2. Start a recording. [to confirm: button or hotkey]
3. Speak normally; Whisplet transcribes and labels speakers as the meeting happens.
4. [to confirm: how notes are taken or edited during the meeting]
5. End the recording. [to confirm: button or hotkey]
6. Review the transcript, speaker labels and notes. [to confirm: where these appear after the
   meeting]

## Where your data lives

Recordings, transcripts, speaker labels and notes are created and kept in a folder on your
computer, one you can open and delete yourself. Whisplet has no account system.

- Default folder: [to confirm: default data folder path]
- How to change it: [to confirm: setting or option, if any]

## What leaves the machine

Whisplet is built to keep meeting content on your computer. The only two things that can
leave your machine are a model download you asked for, and a crash report you chose to send.
Both are described, host by host, at:

https://whisplet.ai/trust

## How to report a bug

Use the bug report form on GitHub Issues in this repository (choose "Bug report" when you
open a new issue). Include:

- Your Whisplet version and build id (shown in Settings).
- Your hardware tier (CPU, NVIDIA, Intel Arc or iGPU, AMD).
- Your Windows version.
- Steps to reproduce, and what you expected versus what happened.
- Error text, a screenshot, or a crash report id if you sent one.

Do not include:

- Transcript text from any meeting.
- Personal data about other people who were in the meeting.

For a feature idea, use the "Feature request" form. For a general question, use the
"Question" form, or start a discussion in Discussions. For anything you do not want to be
public, especially a security issue, mail support@whisplet.ai instead; see SECURITY.md.

## How to send a crash report

If Whisplet crashes, the next time you start it you will see a dialog listing exactly what
it would send: a minidump (crash stack and module list, never audio or transcript text), the
last lines of the application log, and a short version and hardware summary. Nothing is sent
unless you click Send.

After you click Send, the dialog shows a report id. Keep it. If you write to support about the
crash, quote the report id so the maker can find your report.

## How to uninstall and remove all data

The beta is a plain folder, not an installer.

1. Close Whisplet.
2. Delete the folder you unzipped the beta into.
3. Delete your data folder (see "Where your data lives" above) if you want your recordings
   and notes removed as well; Whisplet does not delete this folder for you.

There is no registry entry or background service to remove beyond this. [to confirm: any
other files Whisplet writes outside these two folders, if any]

## Known limitations

This beta build has known rough edges. This list will be kept current during the beta.

- [to confirm: languages or accents with weaker recognition]
- [to confirm: known issues with speaker labels, for example overlapping speech]
- [to confirm: features not yet implemented]
- [to confirm: hardware or driver combinations known not to work]

## Terms and privacy

The beta terms and the privacy page on whisplet.ai apply to your use of this beta:

- https://whisplet.ai/beta
- https://whisplet.ai/privacy
