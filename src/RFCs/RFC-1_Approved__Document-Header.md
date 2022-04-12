# RFC 1 WIP: Document Header

This RFC describes the document header to be used in the doc-chain project.

## The Document Header

The Document Header is the main reference to the original document.
The authenticity of the document contents is proved by the checksum it carries.
It contains the following:

- **Document Reference**: A reference to the document. Probably in the form of a URL or a filename.
- **Document Checksum**: The checksum of the document. SHA-512 recommended.

To prove the authenticity of the document, the document referenced is checked against the checksum.
