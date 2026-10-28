# ChemDraft for Word and PowerPoint

**Status: In development. Nothing to install yet.**

ChemDraft for Word and PowerPoint is a planned Microsoft Office add-in for putting chemical structures drawn in [ChemDraft](https://chemdraft.ai) into Word documents and PowerPoint slides, then editing them again from inside Office. The goal is to select a structure, choose **Edit Structure** on the ribbon, make changes in the ChemDraft editor window, and choose **Done** to replace the picture in its original position and size. **Insert Structure** is intended to add a new structure. This is especially useful on Mac, where Office has no built-in way to edit drawings made in another app from inside a document.

The add-in is planned for Word and PowerPoint on Mac and Windows, and Office on the web. These features are in development and are not available to use yet.

## How it works

Each structure picture is intended to carry the full ChemDraft drawing hidden inside the picture file, so the editable drawing can travel with the document. Structures copied from the ChemDraft desktop app and pasted into Office are also intended to be editable with the add-in. We are still measuring which Office versions keep this hidden data.

## What lives here

This repository will contain the Office side of the add-in: its manifest, ribbon commands, and the small task pane that runs an edit. The ChemDraft editor and the code that reads and writes the hidden drawing are in the [main ChemDraft repository](https://github.com/jgassens/ChemDraft).

## Privacy

The add-in is being designed so that your drawings stay on your computer: ChemDraft will not send them to its servers, and the add-in's own files will be loaded from chemdraft.ai. Your documents are stored wherever Office stores them, such as OneDrive, which is outside ChemDraft's control. A full privacy policy will be published before the add-in is released.

## License

This project is licensed under Apache-2.0. See [LICENSE](LICENSE).
