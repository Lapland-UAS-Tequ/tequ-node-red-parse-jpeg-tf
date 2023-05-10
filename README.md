tequ-node-red-parse-jpeg-tf
=====================

Parse JPEG and extract metadata.

## Install

Run the following command in your Node-RED user directory - typically `~/.node-red`

        npm install Lapland-UAS-Tequ/tequ-node-red-parse-jpeg-tf

## Information

Parses JPEG image and adds metadata to msg.

Supports parsing JPEG images from raw MJPEG stream.

Adds to msg:
 - Basic image info (width,height,size) 
 - Exif data
 - Local timestamp, UTC timestamp, Unix timestamp 
 - Thumbnail of the original image (optional, uses tfjs-node-gpu)
 - Coordinates (if given)
 - Serial number 

 Output message is formatted to Tequ-API compatible format.

Dependencies
- https://flows.nodered.org/node/node-red-contrib-msg-speed
- https://flows.nodered.org/node/node-red-contrib-moment
- https://flows.nodered.org/node/node-red-node-exif
- https://flows.nodered.org/node/node-red-contrib-image-info
- https://www.npmjs.com/package/uuid
- https://www.npmjs.com/package/@tensorflow/tfjs-node-gpu

