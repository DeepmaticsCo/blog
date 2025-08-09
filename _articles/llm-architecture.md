---

layout: post  
title: "Architectural Evolution of Transformers"  
date: 2025-08-01  
image: "assets/llm-architecture/architecture.png"  
excerpt: "Exporing the architectural aspects of how decoder LLMs have imporved and code them."  
author: "Satish Yenumula"  
tags: \[GenAI, Transformers, LLM\]

---

## Introduction

As someone working on GenAI should be well versed with "Transformers architecture" and we would have gone through Jay Alammar's [The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/) explanation that had simplified the "Attnetion Is All You Need" paper.

In this post, we will be go beyond the basics and look at few of the major releases of decoder based large language models and look specifically into the improvements made in an LLM model's architecture. However, from a practitioner standpoint this is not usually the case, a major release that beats benchmarks has multiple aspects to it, including improvements in training data quality, LLM fine-tuning or Preference Tuning methodologies in addition to the architectural changes. However, for the scope of this post, we are only limiting to architectural improvements of a set LLMs, whose information is open-source or the technical reports have been available.

## Foundation and Early Scaling

ChatGPT by OpenAI

<div style="display: flex; align-items: flex-start; margin-bottom: 1em;">
    <div style="flex: 0 0 25%; margin-right: 1em;">
        <a href="{{ site.baseurl }}/assets/llm-architecture/GPT3.png" target="_blank" rel="noopener noreferrer">
            <img src="{{ site.baseurl }}/assets/llm-architecture/GPT3.png" alt="GPT Models" style="width: 100%;" />
        </a>
    </div>
    <div style="flex: 1;">
        <h4>GPT-1</h4>
        <p>-- testing layout</p>
        <p>In this post, we will be go beyond the basics and look at few of the major releases of decoder based large language models and look specifically into the improvements made in an LLM model's architecture. However, from a practitioner standpoint this is not usually the case, a major release that beats benchmarks has multiple aspects to it, including improvements in training data quality, LLM fine-tuning or Preference Tuning methodologies in addition to the architectural changes. However, for the scope of this post, we are only limiting to architectural improvements of a set LLMs, whose information is open-source or the technical reports have been available.</p>
        <h4>GPT-2</h4>
        <p><em>Content for GPT-2 goes here.</em></p>
        <h4>GPT-3</h4>
        <p><em>Content for GPT-3 goes here.</em></p>
    </div>
</div>
<div>
    <p><strong>Code Repo Link:</strong> <em>Link goes here.</em></p>
</div>