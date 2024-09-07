# Cricket Pose Comparison to Enhance Scouting

## Overview
This project aims to revolutionize traditional cricket scouting by using pose estimation technology to compare the techniques of emerging players with those of legendary cricketers. The goal is to generate an objective comparison score based on key shots, providing scouts with a quantifiable metric to evaluate player performance and technical proficiency.

## Motivation
Scouting in cricket has historically relied on subjective visual assessments by scouts, which can introduce personal and professional biases. This project seeks to enhance the accuracy and fairness of player assessments by incorporating data-driven insights. By analyzing the biomechanics of legendary and emerging players across key cricket shots, we aim to create a reliable scoring system that can complement traditional scouting methods.

## Key Features
- **Pose Estimation**: Leverages cutting-edge models like PoseNet and MediaPipe to detect keypoints essential for various cricket shots.
- **Pose Comparison**: Utilizes comparison metrics such as Cosine Similarity, Euclidean Distance, Dynamic Time Warping, and MatchPose to evaluate pose similarity.
- **Comprehensive Shot Analysis**: Focuses on 10 key cricket shots, including cover drive, defense, flick, hook, pull shot, and more.
- **Player Benchmarking**: Uses videos of legendary cricketers as benchmarks to evaluate emerging talent.

## Dataset
The **CricShot10** dataset is used to train and evaluate the pose estimation and comparison models. This dataset contains videos of players performing 10 different cricket shots, with labeled key points for pose analysis.

## Methodology
1. **Object Detection**: Uses **YOLOv8** to detect and crop batsmen from cricket videos, eliminating background noise.
2. **Pose Estimation**: Passes the cropped videos through pose estimation models like PoseNet or MediaPipe to capture keypoints.
3. **Pose Comparison**: Compares player poses using the selected comparison algorithm (Cosine Similarity, Euclidean Distance, etc.) to generate a performance score.
4. **Shot Benchmarking**: Compares emerging players’ shot performance against the benchmark players (e.g., Virat Kohli for cover drives, Sachin Tendulkar for straight drives).

## Results
The scoring system generates values between 0 (worst performance) and 1 (best performance) based on pose similarity with benchmark players.

## Technologies Used
- **PoseNet**, **MediaPipe**, and other advanced Pose Estimation models for keypoint detection
- **YOLOv8** for object detection and background removal
- **Pose Comparison Algorithms**: Cosine Similarity, Euclidean Distance, Dynamic Time Warping, MatchPose

## Performance Analysis
- **Validation**: Compare poses from identical videos (1 vs. 1) and different videos of the same shot (1 vs. many).
- **Scoring**: Generate a comparison score for each shot, providing a clear metric for scouts.

## Future Work
- Improve data quality by gathering higher-resolution videos of both legendary and emerging players.
- Explore 3D pose estimation techniques for more accurate comparison across various dimensions.
  
## Contributors
- **Shreyas Srinivasan** 

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


Model Drive Link: https://drive.google.com/file/d/132A_4eCORgmsRmBdakQ3f8jveb9TvnzT/view?usp=sharing
