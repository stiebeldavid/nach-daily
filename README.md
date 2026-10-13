# Nach Daily

Yonah Klein's daily Nach shiur recordings, shared in the "Nach Daily" WhatsApp group from August 2021 to October 2026. This repository is a complete copy of the group's WhatsApp export ("WhatsApp Chat - Nach Daily.zip"), kept here as permanent storage. Private: these are Yonah's recordings and have not been cleared for publishing.

## What's here

- `audio/` — 1,592 voice recordings (1,590 `.opus` and 2 `.m4a`), original WhatsApp file names. The name carries the date and time sent, e.g. `00000006-AUDIO-2021-08-26-09-58-10.opus` = 26 Aug 2021, 09:58:10.
- `media/` — the other attachments from the chat: 47 `.jpg`, 4 `.webp`, 2 `.mp4`, 1 `.docx`.
- `_chat.txt` — the full chat text from the export, which shows the message posted with each recording.
- `nach_daily_index.csv` — one row per recording: `file`, `date`, `sender`, `bytes`, `est_minutes`, and `chat_label` (the text Yonah posted with it, usually the sefer/perek/pasuk). Use it to find a shiur by sefer, perek or pasuk.

Coverage includes Tehillim 66–150, Mishlei, Shir Hashirim, Iyov, Rus, Eichah, Daniel, Ezra, Nechemya, Divrei Hayamim, Yehoshua through Yechezkel, and Trei Asar up to Zechariah 5. Tehillim 1–62 (a different chat) and Koheles are not in this export.

## Two large recordings stored in parts

Two `.m4a` files were too large for the upload route used, so each is stored as exact byte-for-byte parts:

- `audio/00002562-AUDIO-2024-12-18-09-17-59.m4a` (22,849,541 bytes) is stored as 10 parts, `audio/00002562-AUDIO-2024-12-18-09-17-59.m4a.part01` … `.part10`. Rejoin with:
  `cat audio/00002562-AUDIO-2024-12-18-09-17-59.m4a.part* > audio/00002562-AUDIO-2024-12-18-09-17-59.m4a`
  SHA-256 of the rejoined file: `36cdf41608664ae70d6c0a677848d21be8d69d983f533a100a5efdd45a5c2d4c`
- `audio/00003242-AUDIO-2026-03-01-10-02-19.m4a` (12,105,895 bytes) is stored as 5 parts, `audio/00003242-AUDIO-2026-03-01-10-02-19.m4a.part01` … `.part05`. Rejoin with:
  `cat audio/00003242-AUDIO-2026-03-01-10-02-19.m4a.part* > audio/00003242-AUDIO-2026-03-01-10-02-19.m4a`
  SHA-256 of the rejoined file: `5434619b6265018555a15032708455489c815cc38e3af55ed551a79496d7c457`

## Verification

Every file was copied straight from the export zip and checked: each file's zip CRC was checked when read, and GitHub's content hash of each uploaded file matched the hash of the original bytes. Copied October 2026.
