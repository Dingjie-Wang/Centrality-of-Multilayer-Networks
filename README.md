# The operating instruction of ENMNFinder software

To make other researchers more convenient for identifying essential nodes in multilayer networks, we present a visual software based on GUI of MATLAB, called ENMNFinder (Essential Nodes of Multilayer Networks Finder). The ENMNFinder provides an easy and accessible user interface for the calculation of centralities, and the visual representation of the results of calculations in multilayer networks. In the following, we give technical details about the ENMNFinder software. Here we use the C.elegans multilayer connectome network [1-2] as a test example, and it’s data is available at http://deim.urv.cat/~manlio.dedomenico/data.php.

## 1. The installation of the ENMNFinder software

ENMNFinder software should run under Windows. Depending on two different windows operating systems, two different ENMNFinder softwares are provided for 32-bits and 64-bits, named by ENMNFinder_32_bits and ENMNFinder_64_bits, respectively. Choose the appropriate version according to the different windows operating systems. Before installing the ENMNFinder software, please install the MATLAB Compiler Runtime (MCR) firstly. It is available at http://www.mathworks.com/products/compiler/mcr/index.html. If you use the ENMNFinder_32-bits software, you should choose the version R2012a(7.17) of MCR on 32-bit windows operating system. And if you use the ENMNFinder_64-bits software, you should choose the version R2013a(8.1) of MCR on 64-bit windows operating system. Next, running the ENMNFinder software (ENMNFinder_32_bits.exe or ENMNFinder_64_bits.exe) and the following initialization user interface can be obtained. 

![image](https://github.com/Dingjie-Wang/Centrality-of-Multilayer-Networks/blob/master/fig1.jpg)

## 2. Format of input data

Clicking the button “Input data” in the left enter into the user interface of input data, and you need to input a TXT file. The TXT file contains four column data, which provides the interaction relationships of nodes in multilayer networks, the format is as follows.

![image](https://github.com/Dingjie-Wang/Centrality-of-Multilayer-Networks/blob/master/fig2.jpg)

## 3. The visual representation of the ranking results of centrality methods

Clicking the button “Ranking” in the left enter into the following user interface. In this interface, you can choose different centrality methods (include EDCPTD, eigenvector, PageRank, degree, in-degree, out-degree, hub and authority centralities) to identify essential nodes in multilayer networks, and ranking results of centrality methods can be stored in an XLS file and represented in the following user interface.

![image](https://github.com/Dingjie-Wang/Centrality-of-Multilayer-Networks/blob/master/fig3.jpg)

For example, in the C.elegans multilayer connectome network, we choose authority and EDCPTD centralities to identify essential nodes, the ranking results of two centrality methods are shown in the following interface.

![image] (https://github.com/Dingjie-Wang/Centrality-of-Multilayer-Networks/blob/master/fig4.jpg)

## 4. The visual representation of correlation analysis between different centrality methods

Clicking the button “Correlation” in the left enter into the user interface of correlation analysis. In this interface, you need to choose two different centrality methods. The ENMNFinder can calculate the Spearman correlation between two different centrality methods. For example, in the C.elegans multilayer connectome network, we choose PageRank and degree centralities to identify essential nodes. The value of Spearman correlation between PageRank and degree centralities and corresponding visual figure are shown in the following interfaces.

![image] (https://github.com/Dingjie-Wang/Centrality-of-Multilayer-Networks/blob/master/fig5.jpg)

![image] (https://github.com/Dingjie-Wang/Centrality-of-Multilayer-Networks/blob/master/fig6.jpg)
