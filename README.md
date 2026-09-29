# Raw Material Yard V1.9 — Mobile Field App

## What is upgraded
- Google Apps Script sync remains preconfigured.
- OCR marking: original + contrast + threshold preprocessing, then automatic OCR.
- OCR token chips: tap a recognized code fragment to search.
- Exact search first; fuzzy matching is used when exact results are not found.
- Rich Material Detail: Plate, Heat, Coil, Grade, Specification, Size, Qty, Weight, Project, PO, Yard, Manufacturer, MTC, MRIR, inspection date and remark.
- Camera barcode/QR scan + Capture to OCR.
- Offline cache is retained on the device.

## Current Apps Script endpoint
`https://script.google.com/macros/s/AKfycbwCF_ukyCNhwJzt9Hy9DLxXN2Ps1gh8SubrFp0rcJ2WWbLkr80jjPisoUk9B-yBYpoA/exec`

## Hosting
Upload the **contents of this folder** to the root of GitHub Pages. The expected URL is:
`https://nguyenthao960417.github.io/raw-material-yard/`

## Daily flow
PC: RM_Material.xlsx → Refresh Excel → Publish to Drive

Phone: Open Raw Material Yard → Refresh Data → Search / Scan / Check

## Important
The Apps Script Web App must point to the current `mobile_master.json` File ID:
`1vamlDYhXr3V-rc3x23qW_5i_eCFQP7oJ`

If you changed `Code.gs`, redeploy the Web App before testing mobile sync.
