---
title: Course Description for AI for Mechanical Engineers
description: A detailed course description for AI for Mechanical Engineers including overview, topics covered and learning objectives in the format of the 2001 Bloom Taxonomy
quality_score: 100
---

# AI for Mechanical Engineers

**Title:** AI for Mechanical Engineers

**Target Audience:** College undergraduate — first-year (freshman) mechanical engineering students

**Prerequisites:** High school algebra, trigonometry, and precalculus; high school physics. Calculus I may be taken concurrently. No programming experience is assumed — the book teaches the Python it needs as it goes.

## Course Overview

Generative AI tools are already on every engineering student's laptop, and they
will be standard equipment in every engineering office these students join. Most
first-year students meet these tools with no mental model of how they work, when
they fail, or how an engineer is supposed to check their output. This course
gives freshman mechanical engineers that mental model early — before bad habits
form — and grounds it in the kinds of problems they will see in statics,
dynamics, materials, design, and manufacturing courses.

The course starts with what AI is and is not, then builds just enough data
literacy, statistics, and Python to make machine learning concrete: fitting a
model to lab data, classifying parts as pass or fail, and judging whether a
model is any good. From there it explains, intuitively and without heavy math,
how neural networks and large language models work. The largest part of the
course is practical generative AI for engineering work: writing effective
prompts, verifying AI answers against hand calculations and units, using AI
coding assistants to build engineering scripts, and understanding how AI is
showing up in CAD, generative design, simulation, manufacturing, and
maintenance.

Throughout, the emphasis is on engineering judgment. An engineer signs their
name to their work; AI does not change that. Students finish able to use AI as
a fast, capable assistant while knowing exactly where its answers need to be
checked — and when not to use it at all.

## Main Topics Covered

1. **What AI is (and isn't)** — definitions, a short history, narrow vs.
   general AI, machine learning vs. rule-based systems, and where AI already
   appears in mechanical engineering practice.
2. **Python and Jupyter for engineers** — variables, lists, loops, functions,
   NumPy arrays, plotting with Matplotlib, reading CSV data with pandas, and
   working in notebooks.
3. **Engineering data and statistics** — sensors and measurement, units,
   significant figures, measurement error, data cleaning, visualization,
   mean/variance/standard deviation, distributions, and correlation vs.
   causation.
4. **Machine learning fundamentals** — features and labels, supervised vs.
   unsupervised learning, linear regression on experimental data, classification
   (pass/fail, failure mode), train/test splits, overfitting, error metrics, and
   clustering.
5. **Neural networks, intuitively** — artificial neurons, weights, activation
   functions, layers, loss functions, training as iterative error reduction, and
   how neural networks scale up to modern AI.
6. **How generative AI and large language models work** — tokens, next-token
   prediction, training data, transformers at a conceptual level, context
   windows, temperature, multimodal models, and why hallucinations happen.
7. **Prompting and verifying AI output for engineering** — prompt structure,
   giving context and constraints, asking for assumptions and units, iterative
   refinement, and verification techniques: hand calculations, order-of-magnitude
   checks, unit analysis, limiting cases, and cross-checking sources.
8. **AI coding assistants for engineering computation** — using AI to write,
   explain, and debug Python; reading and testing generated code; building small
   engineering calculators and data-analysis scripts.
9. **AI in design and simulation** — generative design, topology optimization,
   design-space exploration, optimization basics (objectives, constraints,
   iteration), AI features in CAD tools, and surrogate models that approximate
   slow simulations.
10. **AI in manufacturing and maintenance** — computer-vision quality
    inspection, predictive maintenance from vibration and temperature data,
    anomaly detection, and digital twins at an introductory level.
11. **Ethics, safety, and professional responsibility** — engineering codes of
    ethics, accountability for AI-assisted work, safety-critical systems, bias
    and data quality, intellectual property and confidentiality, academic
    integrity, and environmental cost of AI.

## Topics Not Covered

- Derivations of backpropagation, gradient calculus, or other math beyond
  first-semester calculus
- Building or training large language models from scratch
- Reinforcement learning beyond a brief mention
- Finite element analysis (FEA) and computational fluid dynamics (CFD) theory
- Advanced control theory and robotics kinematics
- Deploying models to production (MLOps, cloud infrastructure)
- Step-by-step training in any specific commercial CAD or simulation product
- Advanced Python software engineering (classes, packaging, testing frameworks)

## Learning Outcomes

After completing this course, students will be able to:

### Remember
*Retrieving, recognizing, and recalling relevant knowledge from long-term memory.*

- Define artificial intelligence, machine learning, deep learning, and
  generative AI, and state how they relate to each other.
- List the main types of machine learning (supervised, unsupervised,
  reinforcement) with one mechanical engineering example of each.
- Recall the core vocabulary of data and models: feature, label, training set,
  test set, parameter, loss, overfitting, token, prompt, hallucination.
- Identify common sensors used in mechanical systems (thermocouples, strain
  gauges, accelerometers, load cells) and what each measures.
- Name the fundamental canons of an engineering code of ethics.

### Understand
*Constructing meaning from instructional messages, including oral, written, and graphic communication.*

- Explain, in plain language, how a large language model produces text by
  predicting the next token, and why that leads to confident but wrong answers.
- Describe how a neural network learns by adjusting weights to reduce error.
- Explain why a model that fits its training data perfectly can still fail on
  new data.
- Interpret plots of experimental data, including scatter plots, histograms,
  and time series from sensors.
- Summarize how generative design, surrogate models, vision inspection, and
  predictive maintenance use AI in mechanical engineering practice.
- Explain why measurement error and data quality limit what any model can learn.

### Apply
*Carrying out or using a procedure in a given situation.*

- Write short Python programs in Jupyter to load, clean, and plot engineering
  data.
- Fit a linear regression to lab data (e.g., spring force vs. displacement) and
  use it to make predictions with units.
- Train and test a simple classifier on part-inspection data using a
  train/test split.
- Write structured prompts that give an AI assistant context, constraints,
  required units, and an expected output format.
- Use an AI coding assistant to generate, explain, and fix Python code for an
  engineering calculation.
- Verify an AI-generated answer using unit analysis, order-of-magnitude
  estimates, and an independent hand calculation.

### Analyze
*Breaking material into constituent parts and determining how the parts relate to one another and to an overall structure or purpose.*

- Distinguish engineering problems suited to AI from those better solved with
  first-principles analysis or a lookup table.
- Diagnose why a model performs poorly by examining its data, features, and
  training vs. test error.
- Break an AI-generated solution into its stated assumptions, equations, and
  numerical steps to locate errors.
- Compare residual plots and error metrics across several candidate models.
- Trace how bias or gaps in training data could produce unsafe outputs in a
  mechanical system.

### Evaluate
*Making judgments based on criteria and standards through checking and critiquing.*

- Judge whether an AI-generated calculation, code snippet, or design
  recommendation is trustworthy enough to use, and justify the decision.
- Critique an AI-assisted engineering report for unverified claims, missing
  units, and unstated assumptions.
- Assess the ethical, safety, intellectual-property, and confidentiality risks
  of using AI tools on a given engineering task.
- Select an appropriate model and evaluation metric for a given engineering
  dataset and defend the choice.
- Evaluate competing AI-generated design alternatives against engineering
  requirements (strength, weight, cost, manufacturability).

### Create
*Putting elements together to form a coherent or functional whole; reorganizing elements into a new pattern or structure.*

- Build a small Python engineering tool (e.g., a beam-deflection or
  heat-loss calculator) with the help of an AI coding assistant, including
  tests that check it against hand calculations.
- Design a personal, documented workflow for using AI on engineering homework
  and projects that meets academic-integrity and verification standards.
- Develop a predictive model from a collected or provided dataset and present
  its accuracy and limitations.
- **Capstone project:** Choose a real mechanical engineering problem (e.g., a
  bracket design, a predictive-maintenance alert for a fan, or a 3D-printing
  defect detector), use AI tools to explore solutions, independently verify the
  results, and produce a short engineering report that documents the prompts,
  the verification steps, the final design or model, and an ethics and safety
  review.
