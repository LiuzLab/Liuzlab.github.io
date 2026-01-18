---
title: "MARRVEL-MCP: A Context-Engineered Natural-Language Query-to-Response Interface for Mendelian Disease Discovery"
authors: ["Zachary Everton", "Jorge Botas", "Seon Young Kim", "Zhandong Liu", "Hyun-Hwan Jeong"]
year: 2025
venue: "Unknown Venue"
type: "paper"
cover: "../../assets/paper-vision.jpg"
links:
  pdf: "http://biorxiv.org/lookup/doi/10.1101/2025.11.26.690887"
  code: ""
  website: ""
  demo: ""
  slides: ""
  video: ""
doi: "10.1101/2025.11.26.690887"
description: "A 
            bstract 
           
          Rare disease variant interpretation requires navigating multiple genomic databases with strict input formats and synthesizing heterogeneous evidence, creating barriers for non-experts and cognitive burdens even for specialists. MARRVEL exemplifies this challenge by requiring precise queries (e.g., HGVS notation) and returning complex, difficult-to-synthesize outputs. To address this input-output asymmetry, we developed MARRVEL-MCP, a natural language interface enabling large language models (LLMs) to perform end-to-end variant interpretation via structured tool access. 
           
            This work demonstrates the impact of 
            context engineering 
            —the deliberate design of domain-aware tool environments and information scaffolding—in reshaping the role of model scale in genomics. MARRVEL-MCP equips LLMs with 39 tools spanning gene and variant utilities, pathogenicity databases, phenotype resources, expression atlases, ortholog data, and literature APIs. Without hard-coded pipelines, LLMs autonomously infer workflows, performing named-entity recognition, identifier normalization, and multi-database synthesis from narrative queries. 
           
          Using 45 expert-curated questions, lightweight models (3B–20B parameters) with MARRVEL-MCP matched or outperformed larger models lacking tool access. A 20B-parameter model (gpt-oss-20b) achieved a 95\% pass rate versus 33\% without MARRVEL-MCP, approaching state-of-the-art proprietary performance. Although accuracy remains below the 100\% required for autonomous diagnosis and token usage is considerable, these results show that well-designed context can compensate for limited model capacity. 
           
            These findings establish context engineering as a core principle for biomedical AI, enabling efficient, scalable integration of LLMs with curated genomic resources. MARRVEL-MCP is available at 
            https://github.com/hyunhwan-bcm/MARRVEL\_MCP/ 
            ."
featured: false
---
A 
            bstract 
           
          Rare disease variant interpretation requires navigating multiple genomic databases with strict input formats and synthesizing heterogeneous evidence, creating barriers for non-experts and cognitive burdens even for specialists. MARRVEL exemplifies this challenge by requiring precise queries (e.g., HGVS notation) and returning complex, difficult-to-synthesize outputs. To address this input-output asymmetry, we developed MARRVEL-MCP, a natural language interface enabling large language models (LLMs) to perform end-to-end variant interpretation via structured tool access. 
           
            This work demonstrates the impact of 
            context engineering 
            —the deliberate design of domain-aware tool environments and information scaffolding—in reshaping the role of model scale in genomics. MARRVEL-MCP equips LLMs with 39 tools spanning gene and variant utilities, pathogenicity databases, phenotype resources, expression atlases, ortholog data, and literature APIs. Without hard-coded pipelines, LLMs autonomously infer workflows, performing named-entity recognition, identifier normalization, and multi-database synthesis from narrative queries. 
           
          Using 45 expert-curated questions, lightweight models (3B–20B parameters) with MARRVEL-MCP matched or outperformed larger models lacking tool access. A 20B-parameter model (gpt-oss-20b) achieved a 95\% pass rate versus 33\% without MARRVEL-MCP, approaching state-of-the-art proprietary performance. Although accuracy remains below the 100\% required for autonomous diagnosis and token usage is considerable, these results show that well-designed context can compensate for limited model capacity. 
           
            These findings establish context engineering as a core principle for biomedical AI, enabling efficient, scalable integration of LLMs with curated genomic resources. MARRVEL-MCP is available at 
            https://github.com/hyunhwan-bcm/MARRVEL\_MCP/ 
            .