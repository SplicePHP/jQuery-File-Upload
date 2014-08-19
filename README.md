##Fork of BlueImp's File upload


The primary reason for this fork is to get requirejs to play nice with my general projects.
Only the define methods have been modified in order to allow for propper loading of dependencies.

Should be called via grunt's bower-task library

## Example config
```
requirejs.config({
	paths: {
		"jquery": "lib/jquery/jquery.min",
		"jquery-ui": "lib/jquery-ui/",
		"bi-tmpl": "lib/blueimp-tmpl/tmpl",
		"bi-load-image": "lib/blueimp-load-image/load-image",
		"bi-canvas-to-blob": "lib/blueimp-canvas-to-blob/canvas-to-blob",
		"bi-fileupload-ui": "lib/blueimp-file-upload/jquery.fileupload-ui",
		"bi-fileupload": "lib/blueimp-file-upload/jquery.fileupload",
		"jquery.ui.widget": "lib/blueimp-file-upload/jquery.ui.widget",
		"jquery.iframe-transport": "lib/blueimp-file-upload/jquery.iframe-transport",
		"bi-image": "lib/blueimp-file-upload/jquery.fileupload-image",
		"bi-audio": "lib/blueimp-file-upload/jquery.fileupload-audio",
		"bi-video": "lib/blueimp-file-upload/jquery.fileupload-video",
		"bi-validate": "lib/blueimp-file-upload/jquery.fileupload-validate",
		"bi-fileupload-process": "lib/blueimp-file-upload/jquery.fileupload-process",
		"bi-load-image": "lib/blueimp-load-image/load-image",
		"bi-load-image-meta": "lib/blueimp-load-image/load-image-meta",
		"bi-load-image-exif-map": "lib/blueimp-load-image/load-image-exif-map",
		"bi-load-image-exif": "lib/blueimp-load-image/load-image-exif",
		"bi-load-image-ios": "lib/blueimp-load-image/load-image-ios",
		"bi-load-image-orientation": "lib/blueimp-load-image/load-image-orientation"
	}
})

require(
    [
        'jquery',
        'bi-tmpl',
        'bi-load-image',
        'bi-canvas-to-blob',
        'jquery.iframe-transport',
        'bi-fileupload-ui'
    ],
    function() {
        $('#fileupload').fileupload({
            url: 'server/php/'
        });
    }
);
```
