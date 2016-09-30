FROM alpine:latest
MAINTAINER awmyhr <awmyhr@gmail.com>

# add bash to run imagemagick scripts
# add bc cuz some of Fred Weinhaus' scripts require it
# add ghostscript-fonts as some imagemagick commands throw errors w/out it

RUN apk --no-cache add \
    bash \
    bc \
    ghostscript-fonts \
    imagemagick

# add imagemagick scripts

COPY scripts/createColormap.sh /usr/local/bin

# give a default usage message

CMD [ "echo", "Provides the Image Magick commands animate, compare, composite, conjure, convert, display, identify, import, mogrify, montage, and stream "]
