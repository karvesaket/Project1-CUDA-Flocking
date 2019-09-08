**University of Pennsylvania, CIS 565: GPU Programming and Architecture,
Project 1 - Flocking**

* Saket Karve
  * [LinkedIn](https://www.linkedin.com/in/saket-karve-43930511b/), [twitter](), etc.
* Tested on:  Windows 10 Education, Intel(R) Core(TM) i7-6700 CPU @ 3.40GHz 16GB, NVIDIA Quadro P1000 @ 4GB (Moore 100B Lab)


### Sample Outputs
1. Naive

**Configuration**: Number of boids = 50,000 | Block Size = 128 | Cell width = 2 x max_distance
![]()

2. Uniform Grid

**Configuration**: Number of boids = 50,000 | Block Size = 128 | Cell width = 2 x max_distance
![]()

3. Unifirm Grid with coherent arrays

**Configuration**: Number of boids = 50,000 | Block Size = 128 | Cell width = 2 x max_distance
![]()

### Performance Analysis

Performance is measured in terms of Frames per second (fps) as an estimate of the average fps value observed after running with different configurations.

#### Effect of changing number of boids

Other fixed parameters: Block size = 128; Cell width = 2 x max_disatnce

| With visualization | Without visualization |
| -------------------|---------------------- |
| ![]()              | ![]()                 |

#### Effect of changing block size (number of threads per block)

Other fixed parameters: Number of boids = 5,000; Cell width = 2 x max_disatnce

| With visualization | Without visualization |
| -------------------|---------------------- |
| ![]()              | ![]()                 |

Other fixed parameters: Number of boids = 100,000; Cell width = 2 x max_disatnce

| With visualization | Without visualization |
| -------------------|---------------------- |
| ![]()              | ![]()                 |

#### Effect of changing cell width (number of cells)

Other fixed parameters: Number of boids = 5,000; Block size = 128

| With visualization | Without visualization |
| -------------------|---------------------- |
| ![]()              | ![]()                 |

#### Answers to questions

* For each implementation, how does changing the number of boids affect performance? Why do you think this is?
  * ANSWER

* For each implementation, how does changing the block count and block size affect performance? Why do you think this is?
  * ANSWER

* For the coherent uniform grid: did you experience any performance improvements with the more coherent uniform grid? Was this the outcome you expected? Why or why not?
  * ANSWER

* Did changing cell width and checking 27 vs 8 neighboring cells affect performance? Why or why not? Be careful: it is insufficient (and possibly incorrect) to say that 27-cell is slower simply because there are more cells to check!
  * ANSWER

#### General trend and conclusion
