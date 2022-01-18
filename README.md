# [/r/anime](https://www.reddit.com/r/anime) Comment Face Assets

The repository of media and data of [/r/anime](https://www.reddit.com/r/anime) Comment Faces.

## Directory Structure
* `preview`
  Comment Faces in the dimensions used by the [/r/anime](https://www.reddit.com/r/anime) stylesheet. They're previews for how the Comment Faces will look on the subreddit after being manually processed and embedded into the set of pre-stitched spritesheets found [here](https://github.com/r-anime/stylesheet/tree/main/images).
  * `active`
    The set of currently active Comment Faces.
  * `discontinued`
    The set of discontinued Comment Faces.
* `source`
  * `animated`
    The source frames for the animated Comment Faces. Each directory represents a Comment Face. The frames are stored as PNG images named as 4-digit numbers starting from 0.
    * `original`
    Each directory may contain a subdirectory containing the original file that the source is created from.
    * `edited`
    Each directory may contain a subdirectory containing an edited version of the original file that the source is created from.
  * `static`
    The source images of the static Comment Faces. Each directory represents a Comment Face. The images are stored as PNG files named after the Comment Face.
    * `original`
    Each directory may contain a subdirectory containing the original file that the source is created from.
    * `edited`
    Each directory may contain a subdirectory containing an edited version of the original file that the source is created from.

## List of Comment Faces

The data about the Comment Faces are stored in `comment_face_list.csv` with following fields:
* `name` - Name of the Comment Face (used in the link).
* `is_animated` - Whether the Comment Face is animated.
* `source_width` - The initial width of the source image(s).
* `source_height` - The initial height of the source image(s).
* `resized_width` - The width of the image(s) after resizing.
* `resized_height` - The height of the image(s) after resizing.
* `crop_top` - The number of pixels cropped from the top.
* `crop_bottom` - The number of pixels cropped from the bottom.
* `crop_left` - The number of pixels cropped from the left.
* `crop_right` - The number of pixels cropped from the right.
* `output_width` - The width of the image(s) after cropping.
* `output_height` - The height of the image(s) after cropping.
* `frame_count` - The number of frames (animated only).
* `duration_s` - The duration in seconds (animated only).
* `is_loop` - Whether the animation is looped (animated only).
* `released_on` - The date when the Comment Face was released.
* `discontinued_on` - The date when the Comment Face was discontinued.
* `notes` - Notes related to the Comment Face processing.
