---
layout: post
title: Cryptography
subtitle: by twl
gh-repo: tianwenlong001/tianwenlong001.github.io
gh-badge: [star, fork, follow]
tags: [learning]
comments: true
---

- [LWE](#lwe)
- [Homomorphic Encryption](#homomorphic-encryption)
- [Zero-Knowledge Proof](#zero-knowledge-proof)
- [Crypto Analysis](#crypto-analysis)
- [ASCON](#ascon)


#### LWE

https://github.com/josephsurin/lattice-based-cryptanalysis

https://github.com/Art3misOne/rlwe

https://mysite.science.uottawa.ca/mnevins/papers/StephenHarrigan2017LWE.pdf

https://cseweb.ucsd.edu/classes/fa17/cse206A-a/LecFHE.pdf

https://eprint.iacr.org/2023/032.pdf

https://arxiv.org/pdf/2312.06951.pdf

https://sphincs.org



####  Homomorphic Encryption


####  Zero-Knowledge Proof


#### Crypto Analysis


https://www.cnblogs.com/cway/p/15464406.html

实验metrics https://www.cnblogs.com/cway/p/15464406.html

https://wumansgy.github.io/2018/11/03/AES的CTR模式加密解密详解/

https://zhuanlan.zhihu.com/p/78913397

https://blog.csdn.net/Chahot/article/details/124940142

https://asecuritysite.com/hash/spongent2


#### ASCON

思路：Initialization阶段找到相关密钥，使得中间结果相同，后面的iteration和finalization都是一样的

不容易，要找128bit的原像



eBAC  Ecrypt benchmarking

https://bench.cr.yp.to

0.55 cycles per byte



Cube,

碰撞、

原像、MITM

抗量子  FSE  dongxiaoyang  密钥恢复