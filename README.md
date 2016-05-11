# Parallel BGP Simulation

Border Gateway Protocol simulation using parallel computing techniques.

This project is intendedto the build a parallel Border Gateway Protocol (BGP) simulation system that can simulate BGP routing decision making procedure in real-time for all autonomous systems (ASes) on the Internet.
There are about 60,000 ASes, constructing complex inter-connection networks. 
Each AS make decision on whether to propagate a route upon receiving an BGP announcement. 
The propagation should eventually reach all ASes on the Internet, making every AS knows where to forward the traffic toward every IP address blocks.

Initial idea of the implementation is through MPI. 
The main challenge is the topology information is a huge 60,000 by 60,000 matrix (about 20GB uncompressed), 
which could be quite a challenge to share among the computing nodes. 

Here is a list of academic paper on this topic.

* Dimitropoulos, X. a, Riley, G. F., Georgia, E. C. E., & Atlanta, T. (2004). Large – Scale Simulation Models of BGP.
* Dimitropoulos, X. a., & Riley, G. F. (2006). Efficient large-scale BGP simulations. Computer Networks, 50(12), 2013–2027. http://doi.org/10.1016/j.comnet.2005.09.033
* Coudert, D., Hogie, L., Lancin, A., Papadimitriou, D., Perennes, S., & Tahiri, I. (2012). Feasibility study on distributed simulations of BGP. In Proceedings - 2012 ACM/IEEE/SCS 26th Workshop on Principles of Advanced and Distributed Simulation, PADS 2012 (pp. 96–98). http://doi.org/10.1109/PADS.2012.19
* Liu, Y., Szymanski, B. K., & Saifee, A. (2006). Genesis: A scalable distributed system for large-scale parallel network simulation. Computer Networks, 50(12), 2028–2053. http://doi.org/10.1016/j.comnet.2005.10.002
* Nicol, D. M., Smith, S. W., & Zhao, M. (2004). Evaluation of efficient security for BGP route announcements using parallel simulation. Simulation Modelling Practice and Theory, 12(3-4 SPEC. ISS.), 187–216. http://doi.org/10.1016/j.simpat.2003.10.003
* Nguyen, H., Roughan, M., Knight, S., Falkner, N., Maennel, O., & Bush, R. (2011). How to build complex, large-scale emulated networks. In Lecture Notes of the Institute for Computer Sciences, Social-Informatics and Telecommunications Engineering, LNICST (Vol. 46, pp. 3–18). http://doi.org/10.1007/978-3-642-17851-1_1
* Yocum, K., Eade, E., Degesys, J., Becker, D., Chase, J., & Vahdat, A. (n.d.). Toward Scaling Network Emulation using Topology Partitioning.
* Szymanski, B. K., Liu, Y., & Gupta, R. (2003). Parallel network simulation under distributed Genesis. In Proceedings - 17th Workshop on Parallel and Distributed Simulation, PADS 2003 (pp. 61–68). http://doi.org/10.1109/PADS.2003.1207421
