### ImageJ and Python based Particle Counter
As a part of my master's thesis work, I have process images and count number of clusters of different sizes. A cluster of size `4` denotes that the cluster has `4` particles. Suppose we have a image of plattinum coated silica particles which has many clusters of particles. Each cluster could of different size. Our goal is to count the number of clusters of size `1`, `2`, `3`, `4`, `5`, and `>5`.
## Methodology
1. ImageJ is a Java-based image processing program. First, we we use ImageJ to process the image. Then we find the area of each cluster in our image. We export that as a `.csv` files.
2. Now, we based on the image and areas, we find the area of a single particle by careful eyeballing.
3. Now, we use `Pandas`, `Numpy` of Python and read all the `.csv` we have. Then using the area of the single particle, we find the number of clusters of size size `1`, `2`, `3`, `4`, `5`, and `>5`. For example, a cluster of size `3` will have thrice the area of the single particle.
4. Next, we plot all the result.
