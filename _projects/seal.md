---
layout: post
title: SEAL
feature-img: "assets/img/projects/seal.png"
img: "assets/img/projects/seal.png"
date: 01 September 2017
tags:
---

Side channel attacks use, alongside information such as plaintexts or ciphertexts, leakage about the (secret) key-dependent intermediate state(s), and deliver a  key ranking as a result. Many published works showed that for many practical implementations, observing a few encryptions made complete key recovery possible in practice. The academic research into combating these attacks so far has largely focused on approaches and tools to equip specialised cryptographic engineers with access to a specialist lab and tools.

The research hypothesis of this research project is that one can make meaningful statements about the leakage behaviour of arbitrary implementations on small devices by utilising a-priori derived (instruction level) leakage models. Our vision is to enable developers with limited domain-specific knowledge to perform side channel evaluations at design time without access to a fully equipped lab, by creating tools and methodologies that integrate a priori derived instruction-level leakage models into a standard compiler.

So far this project has produced the following outputs:

- ELMO: an instruction leakage simulator for the ARM M0 family. Source code is provided [here](http://www.github.com/sca-research/elmo). There is an associated [paper](https://www.usenix.org/system/files/conference/usenixsecurity17/sec17-mccann.pdf) that details the novel modelling technique that is based on the SEAL proposal. We used ELMO in our research on implementation options and attacks for the post quantum scheme Frodo [paper](https://link.springer.com/chapter/10.1007%2F978-3-030-10970-7_10). ELMO was also used as the basis for the REASSURE project. The models that we derived for the M0 implementations made us aware of leakage that leads to devastating attacks on [share slicing](https://tches.iacr.org/index.php/TCHES/article/view/8396) implementations.

- GILES: is an extendable instruction leakage and fault simulation framework. It facilitates the integration of different instruction emulators and leakage models, and allows conducting leakage and fault attacks simultaneously. We provide the source [here](http://www.github.com/sca-research/giles).

- Advanced attack techniques: we studied and improved the use of [belief propagation](https://doi.org/10.1007/978-3-030-15462-2_2) demonstrating how to improve both convergence and effectiveness. Related to this we studied the use of [deep neural nets](https://eprint.iacr.org/2019/1068) instead (or alongside) classical statistical and machine learning classifiers.

This project has received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (grant agreement No 725042).

{% include aligner.html images="LOGO_ERC-FLAG_EU.jpg" %}
