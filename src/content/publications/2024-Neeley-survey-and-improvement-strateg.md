---
title: "Survey and improvement strategies for gene prioritization with large language models"
authors: ["Matthew B Neeley", "Guantong Qi", "Guanchu Wang", "Ruixiang Tang", "Dongxue Mao", "Chaozhong Liu", "Sasidhar Pasupuleti", "Bo Yuan", "Fan Xia", "Pengfei Liu", "Zhandong Liu", "Xia Hu"]
year: 2024
venue: "Bioinformatics Advances"
type: "paper"
cover: "../../assets/paper-vision.jpg"
links:
  pdf: "https://academic.oup.com/bioinformaticsadvances/article/doi/10.1093/bioadv/vbaf148/8172498"
  code: ""
  website: ""
  demo: ""
  slides: ""
  video: ""
doi: "10.1093/bioadv/vbaf148"
description: "Abstract 
             
              Motivation 
              Rare diseases remain difficult to diagnose due to limited patient data and genetic diversity, with many cases remaining undiagnosed despite advances in variant prioritization tools. While large language models have shown promise in medical applications, their optimal application for trustworthy and accurate gene prioritization downstream of modern prioritization tools has not been systematically evaluated. 
             
             
              Results 
              We benchmarked various language models for gene prioritization using multi-agent and Human Phenotype Ontology classification approaches to categorize patient cases by phenotype-based solvability levels. To address language model limitations in ranking large gene sets, we implemented a divide-and-conquer strategy with mini-batching and token limiting for improved efficiency. GPT-4 outperformed other language models across all patient datasets, demonstrating superior accuracy in ranking causal genes. Multi-agent and Human Phenotype Ontology classification approaches effectively distinguished between confidently-solved and challenging cases. However, we observed bias toward well-studied genes and input order sensitivity as notable language model limitations. Our divide-and-conquer strategy enhanced accuracy, overcoming positional and gene frequency biases in literature. This framework optimized the overall process for identifying disease-causal genes compared to baseline evaluation, better enabling targeted diagnostic and therapeutic interventions and streamlining diagnosis of rare genetic disorders. 
             
             
              Availability and implementation 
              Software and additional material is available at: https://github.com/LiuzLab/GPT-Diagnosis"
featured: false
---
Abstract 
             
              Motivation 
              Rare diseases remain difficult to diagnose due to limited patient data and genetic diversity, with many cases remaining undiagnosed despite advances in variant prioritization tools. While large language models have shown promise in medical applications, their optimal application for trustworthy and accurate gene prioritization downstream of modern prioritization tools has not been systematically evaluated. 
             
             
              Results 
              We benchmarked various language models for gene prioritization using multi-agent and Human Phenotype Ontology classification approaches to categorize patient cases by phenotype-based solvability levels. To address language model limitations in ranking large gene sets, we implemented a divide-and-conquer strategy with mini-batching and token limiting for improved efficiency. GPT-4 outperformed other language models across all patient datasets, demonstrating superior accuracy in ranking causal genes. Multi-agent and Human Phenotype Ontology classification approaches effectively distinguished between confidently-solved and challenging cases. However, we observed bias toward well-studied genes and input order sensitivity as notable language model limitations. Our divide-and-conquer strategy enhanced accuracy, overcoming positional and gene frequency biases in literature. This framework optimized the overall process for identifying disease-causal genes compared to baseline evaluation, better enabling targeted diagnostic and therapeutic interventions and streamlining diagnosis of rare genetic disorders. 
             
             
              Availability and implementation 
              Software and additional material is available at: https://github.com/LiuzLab/GPT-Diagnosis