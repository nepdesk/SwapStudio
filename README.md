## SwapStudio

SwapStudio is a face-swapping tool for images and videos. It uses a single reference photo to transfer a face onto a target clip or still image, with no dataset and no training required.

This project is inspired by the original roop project and adapted for a new standalone release. Original project: https://github.com/s0md3v/roop

## Installation

Installation can be technical. Make sure you are using the recommended Python version, install the dependencies listed in this repository, and then launch the app or run the headless command from the Usage section.

## Usage

Start the program with arguments:

```
python run.py [options]

-h, --help                                                                 show this help message and exit
-s SOURCE_PATH, --source SOURCE_PATH                                       select an source image
-t TARGET_PATH, --target TARGET_PATH                                       select an target image or video
-o OUTPUT_PATH, --output OUTPUT_PATH                                       select output file or directory
--frame-processor FRAME_PROCESSOR [FRAME_PROCESSOR ...]                    frame processors (choices: face_swapper, face_enhancer, ...)
--keep-fps                                                                 keep target fps
--keep-frames                                                              keep temporary frames
--skip-audio                                                               skip target audio
--many-faces                                                               process every face
--reference-face-position REFERENCE_FACE_POSITION                          position of the reference face
--reference-frame-number REFERENCE_FRAME_NUMBER                            number of the reference frame
--similar-face-distance SIMILAR_FACE_DISTANCE                              face distance used for recognition
--temp-frame-format {jpg,png}                                              image format used for frame extraction
--temp-frame-quality [0-100]                                               image quality used for frame extraction
--output-video-encoder {libx264,libx265,libvpx-vp9,h264_nvenc,hevc_nvenc}  encoder used for the output video
--output-video-quality [0-100]                                             quality used for the output video
--max-memory MAX_MEMORY                                                    maximum amount of RAM in GB
--execution-provider {cpu} [{cpu} ...]                                     available execution provider (choices: cpu, ...)
--execution-threads EXECUTION_THREADS                                      number of execution threads
-v, --version                                                              show program's version number and exit
```

### Headless

Using the `-s/--source`, `-t/--target` and `-o/--output` argument will run the program in headless mode.

## Disclaimer

This software is designed to contribute positively to the AI-generated media industry, assisting artists with tasks like character animation and models for clothing.

We are aware of the potential ethical issues and have implemented measures to prevent the software from being used for inappropriate content, such as nudity.

Users are expected to follow local laws and use the software responsibly. If using real faces, get consent and clearly label deepfakes when sharing. The developers aren't liable for user actions.

## Licenses

Our software uses a lot of third party libraries as well pre-trained models. The users should keep in mind that these third party components have their own license and terms, therefore our license is not being applied.

## Credits

- This repo took inspiration from [s0md3v/roop](https://github.com/s0md3v/roop), the original project that inspired this release.
- This repo also took inspiration from [deepinsight](https://github.com/deepinsight) for their [insightface](https://github.com/deepinsight/insightface) project, which provided a well-made library and models.
- all developers behind the libraries used in this project

## Future Plans

- Build a Flask-based dashboard for easier control and monitoring.
- Add a cleaner web interface for managing source, target, and output files.
- Improve job progress visibility and processing status tracking.

## Documentation

Read the documentation in this repository for setup notes, usage examples, and troubleshooting.
