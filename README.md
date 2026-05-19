# Legacy of Kain: Defiance Remastered - Text Editor Tool

Text editor tool for fan translations of **Legacy of Kain: Defiance Remastered**.

This tool can export the English text from the local game archive into an editable TXT file, and it can import an edited translation TXT back into the local game archive.

## Important

This repository does **not** contain any original game files.

You must own a legitimate copy of **Legacy of Kain: Defiance Remastered**.

## Included files

A release package may contain:

- `LoKDR_Text_Tool_(NooB).exe`
- `Defiance_PCEnglish_TRANSLATE.txt` optional - only if a ready-made translation is being distributed

## Game files

The tool works with the local game archive files in your own game folder.

Required for export and import:

- `bigfile.x64.dat`

## How the tool chooses Export or Import mode

The tool automatically chooses the mode based on whether this file exists next to the EXE:

```
Defiance_PCEnglish_TRANSLATE.txt
```

If the TXT file is **missing**, the tool starts in **Export mode**.

If the TXT file is **present**, the tool starts in **Import mode**.

## Export mode - create an editable translation TXT

Use this mode if you want to create or update a translation file.

1. Open your **Legacy of Kain: Defiance Remastered** game folder.

2. Copy this file into the same folder as `bigfile.x64.dat`:

   - `LoKDR_Text_Tool_(NooB).exe`

3. Make sure this file does **not** already exist in the same folder:

   - `Defiance_PCEnglish_TRANSLATE.txt`

4. Run:

   ```
   LoKDR_Text_Tool_(NooB).exe
   ```

5. The tool will create:

   ```
   Defiance_PCEnglish_TRANSLATE.txt
   ```

6. Open the TXT file and edit only the `TRANSLATION:` lines.

Example:

```
ORIGINAL: Help me...help me...
TRANSLATION: Segíts...segíts...
```

## Import mode - apply an edited translation TXT

Use this mode if you already have a translated TXT file and want to apply it to the game.

1. Open your **Legacy of Kain: Defiance Remastered** game folder.

2. Copy these files into the same folder as `bigfile.x64.dat`:

   - `LoKDR_Text_Tool_(NooB).exe`
   - `Defiance_PCEnglish_TRANSLATE.txt`

3. Make sure these files are in the same folder:

   - `bigfile.x64.dat`
   - `LoKDR_Text_Tool_(NooB).exe`
   - `Defiance_PCEnglish_TRANSLATE.txt`

4. Run:

   ```
   LoKDR_Text_Tool_(NooB).exe
   ```

5. Wait until the process finishes.

When the process is complete, the translation has been applied to `bigfile.x64.dat`.

## Notes for translators

The TXT file uses a simple structure:

```
ORIGINAL: English text
TRANSLATION: Translated text
```

Only edit the text after `TRANSLATION:`.

Do not edit the `ORIGINAL:` lines unless you know exactly what you are doing.

## Antivirus note

This tool is built as a single-file Python executable.

Some antivirus engines may incorrectly flag single-file PyInstaller applications as suspicious because they contain an embedded Python runtime. This is a false positive.

The tool only reads and modifies local **Legacy of Kain: Defiance Remastered** archive files in the same folder.

It does not:

- connect to the internet
- collect personal data
- install background services
- modify system files
- access passwords or browser data

## Restore original files

To restore the original game files, use Steam file verification, or restore your own backup of:

- `bigfile.x64.dat`

The current version of this tool does not modify `bigfilehd.dat`.

## Credits

Tool author: N o o B

## Disclaimer

This is an unofficial fan project.

Legacy of Kain and related names, characters, and assets belong to their respective owners.
