# Fast-Online-Collision-Detection-RRTConnect
Aiming at the problems of low e伍ciency and success rate, high percentage of time-consuming collision detection
in robotic arm path planning within narrow spaces, this paper proposes an online path planning algorithm for narrow spaces
utilizing online fast collision detection in high-dimensional configuration space. The algorithm takes RRTConnect as the
baseline path search framework, and runs the fast collision detection module based on high-dimensional configurations
online clustering in parallel. The module includes balanced sampling of the high-dimensional configuration dataset and
online training of the fast collision detection model. Specifically, in the phase of dataset online construction, a heuristic
strategy is introduced to fully explore the free points in narrow space, overcoming the problem that uniform sampling
leads to an uneven number of collision and free configurations in the dataset, and to provide efective data support for the
subsequent model training; After the dataset construction, the online clustering of collision and free configurations are
used to characterize the distribution of collisions and free configurations in high-dimensional configuration space; Using the
trained cluster model, the collision detection based on bounding box in the baseline algorithm can be transformed into the
calculation of the distance between the sampled configuration and the cluster, which greatly reduces the time consuming
for a single collision detection and efectively improves the e伍ciency of proposed algorithm. Through simulation tests
and experimental verification in simple, opened and closed three types of narrow environment, the results show that the
proposed algorithm has significant advantages in terms of path searching e伍ciency and success rate.
