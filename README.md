<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
***
***
***
*** To avoid retyping too much info. Do a search and replace for the following:
*** github_username, repo_name, twitter_handle, email, project_title, project_description
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <h3 align="center">FasterRCNN</h3>

  <p align="center">
    FasterRCNN implementation in Keras, using Google's Open Image Dataset v6.
    <br />
    <a href="https://github.com/Iarrova/FasterRCNN"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/Iarrova/FasterRCNN">View Demo</a>
    ·
    <a href="https://github.com/Iarrova/FasterRCNN/issues">Report Bug</a>
    ·
    <a href="https://github.com/Iarrova/FasterRCNN/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

FasterRCNN object detection using Keras, trained with Google's Open Image Dataset v6.


### Built With

* [Tensorflow](https://www.tensorflow.org/)
* [Keras](https://keras.io/)
* [OpenCV](https://opencv.org/)


<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* Tensorflow 2.4.0
* Keras 2.4.3
* OpenCV-Python 4.5.1.48
* Numpy 1.19.5
* Pandas 1.1.5
* Scikit-Learn 0.24.0
* Scikit-Image 0.17.2
* Jupyter Notebook 6.1.6

To install prerequisites, simply run:
  ```sh
  pip install -r requirements.txt
  ```


### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/Iarrova/FasterRCNN.git
   ```
2. Install required packages
   ```sh
   pip install -r requirements.txt
   ```



<!-- USAGE EXAMPLES -->
## Usage

DataPreprocessing.ipynb scans Open Image Dataset for the specified classes, download class specific images and creates the files 'train_annotations.txt' and 'test_annotations.txt' with the correct format for training the FRCNN network.

FRCNN_Train_VGG.ipynb loads the annotation files and trains the network, using VGG16 as feature extractor. Creates required files and saves the weights after training.

FRCNN_Test_VGG.ipynb loads the trained model and validates, showing examples of working predictions and calculating mAP (mean Average Precision) score.


<!-- NOTES -->
## Notes
Please do note that the FRCNN_Train_VGG.ipynb trains only for a few epochs. This was for demonstration purposes. The real training was done on Google Colab for 40 Epochs and using 1000 Steps per Epoch. The weights file available under model/ is the one done on Google Colab.


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Ian Roberts  - ian.roberts@sansano.usm.cl

Project Link: [https://github.com/Iarrova/FasterRCNN](https://github.com/Iarrova/FasterRCNN)



<!-- ACKNOWLEDGEMENTS -->
## Acknowledgements

* [README Template](https://github.com/othneildrew/Best-README-Template/)
* [FasterRCNN for Open Images Dataset](https://github.com/RockyXu66/Faster_RCNN_for_Open_Images_Dataset_Keras/)





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/Iarrova/repo.svg?style=for-the-badge
[contributors-url]: https://github.com/Iarrova/repo/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/Iarrova/repo.svg?style=for-the-badge
[forks-url]: https://github.com/Iarrova/repo/network/members
[stars-shield]: https://img.shields.io/github/stars/Iarrova/repo.svg?style=for-the-badge
[stars-url]: https://github.com/Iarrova/repo/stargazers
[issues-shield]: https://img.shields.io/github/issues/Iarrova/repo.svg?style=for-the-badge
[issues-url]: https://github.com/Iarrova/repo/issues
[license-shield]: https://img.shields.io/github/license/Iarrova/repo.svg?style=for-the-badge
[license-url]: https://github.com/Iarrova/repo/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/Iarrova
