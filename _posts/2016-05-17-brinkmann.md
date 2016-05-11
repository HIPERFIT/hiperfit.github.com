---
layout: post
title: "Talk on File System Scalability by André Brinkmann"
category: news
tags: [talk, André Brinkmann]
---
{% include JB/setup %}

## HIPERFIT Seminar Talk

_Title:_ File System Scalability with Highly Decentralized Metadata on Independent Storage Devices

_Presenter:_ André Brinkmann, Johannes Gutenberg Universität, Mainz

_Time:_ Tuesday, May 17, 2016, 15:01-16:00

_Place:_ Universitetsparken 5, Auditorium 10 (mezzanine, south end of building), University of Copenhagen.

## Abstract:

Data handling concepts for Cloud Computing and High-Performance
Computing have been developed nearly independently from each other and
are still mostly restricted to their initial use cases. Cloud
Computing approaches try to scale out by removing the file system
abstraction and applying a flat key-value namespace, while HPC
environments rely on file system semantics and the corresponding
management capabilities. This talk discusses an approach to overcoming
the resulting gap by building a file system with a (very slightly)
relaxed Posix-semantics on top of the key-value interface of the
Seagate Kinetic storage platform. Taking advantage of higher-level
functionality to handle metadata on the drives themselves a
server-less system architecture is proposed. Skipping path component
traversal during the lookup operation is the key technique discussed
in this paper to avoid performance degradation with highly
decentralized metadata. Scalability implications are reviewed based on
a fuse file system implementation.

## Biography

André Brinkmann is full professor at the computer science department
of Johannes Gutenberg University in Mainz, where he heads the
university's data processing center. He received his Ph.D. in
electrical engineering in 2004 from the University of Paderborn, where
he subsequently was assistant professor and managing director of the
Paderborn Centre for Parallel Computing (PC2) from 2008 to 2011. His
research interests focus on algorithm engineering techniques in data
centre management, cloud computing, and storage systems. He has
published more than 100 papers in renowned conferences and journals.
He is associate editor of ACM Transactions on Storage and steering
committee member of French Grid'5000 and the IEEE Symposium on Massive
Storage Systems and Technologies (MSST) and IEEE International
Conference on Networking, Architecture, and Storage (NAS).

All are welcome. No registration required.

_Hosts:_ Fritz Henglein, DIKU, HIPERFIT.
