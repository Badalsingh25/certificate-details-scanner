CERTIFICATE DETAILS SCANNER — SETUP

Files:
- index.html: responsive 3-screen website with camera QR scanner
- sample-certificate-qr.png: QR code containing Badal Singh's certificate details
- certificate-data.json: editable sample QR payload

IMPORTANT:
This is a personal certificate-details viewer. It reads data encoded in the QR code.
It is NOT connected to Infosys, Infosys Springboard, or any certificate issuer and
does NOT independently verify authenticity. The green-style status is intentionally
worded "Certificate Details Retrieved" rather than claiming official verification.

HOW TO TEST:
1. Open the sample-certificate-qr.png on another phone or on a second screen.
2. Open the website on your phone through HTTPS.
3. Tap "Scan QR code" and allow camera access.
4. Point the camera at the sample QR.
5. The certificate details should appear.
6. Tap "Verify Another Certificate" to scan again.

PUBLISH FREE WITH GITHUB PAGES:
1. Create a public GitHub repository (e.g. certificate-details-scanner).
2. Upload index.html to the repository root.
3. Upload sample-certificate-qr.png if you want it available as a test QR.
4. Open Settings > Pages.
5. Choose "Deploy from a branch", branch "main", folder "/ (root)", and Save.
6. Wait for GitHub Pages to publish the HTTPS website URL.

CAMERA REQUIREMENT:
Phone browsers generally require HTTPS (or localhost) for camera access.
Do not test camera access by opening index.html directly as a file.

CREATE ANOTHER CERTIFICATE QR:
Edit certificate-data.json using the same fields, then create a QR code containing
that JSON text. The website expects:
{
  "type": "certificate-details",
  "issuedTo": "...",
  "eventName": "...",
  "startDate": "...",
  "endDate": "...",
  "issuanceDate": "...",
  "certificateId": "..."
}
