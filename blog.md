# Blog
## Exercise 07: Assignment A5
### Topic: Explanations
> **Date:** 11.01.2021 - 02:59 PM *(Due: 11.01.2020 - 03:00 PM)*
> **Name:** `xiyu` (X. Y.) & `goto` (Gorgin T.)
> **Session:** [07 Exercise - Explanations](https://github.com/FUB-HCC/hcds-winter-2020/wiki/07_exercise)   
----

## A5 - Explanations

### Task 1: Different Explanation Needs
> **Goal:** 🥅 &nbsp; Understanding the role-based model by Tomsett et al. and applying it in the context of ORES.

During the lecture ([VL6](https://github.com/FUB-HCC/hcds-winter-2020-slides/blob/main/lecture/06_HCDS_Post-hoc_Interpretability.pdf) and [VL7](https://github.com/FUB-HCC/hcds-winter-2020-slides/blob/main/lecture/07_HCDS_Explanation_Interfaces.pdf)) the role-based Model by Tomsett et al. <sup>[1]</sup> for analyzing interpretable ML system was introduced. The authors defined six roles as follows: Creators, Operators, Executors, Decision-subjects, Data-subjects, and Examiners. (🖼️  https://github.com/FUB-HCC/hcds-winter-2020/blob/main/assignments/A5_Explanation/role-model.png)

1. Please recap the **six roles** and the **example scenarios** by reading the original paper<sup>[1]</sup>. Please read sections `2. Ecosystem model` and section `3. Example scenarios` (pages 9 to 11).
1. Please describe the **roles** and the different **explanation needs** in the context of ORES by writing your own scenario.  (🔲 150 words) **[2 points]** 🔴 🔴 
1. **Reflection:** Please consider yourself as a developer/data scientist using a human-centered design process to develop a new ML system: When would you use this HCI method (role-based model) in your design process and for what reason? (🔲  Illustration + 2-3 sentences)
![](role-model.png) **[2 points]** 🔴 🔴 



#### ORES Scenario
_your TEXT here_

#### Reflection
_your TEXT here_

_your IMAGE here_

### Task 2: Explanation method: LIME
> **Goal:** 🥅 &nbsp; Getting familiar with LIME as an explanation method for evaluating classifiers.

LIME was introduced as a model-agnostic and local explanation/interpretability method in the lecture ([VL6](https://github.com/FUB-HCC/hcds-winter-2020-slides/blob/main/lecture/06_HCDS_Post-hoc_Interpretability.pdf)). We will use the tutorial [Basic usage, two class. We explain random forest classifiers.](https://marcotcr.github.io/lime/tutorials/Lime%20-%20basic%20usage%2C%20two%20class%20case.html) provided in the [LIME repository](https://github.com/marcotcr/lime) on GitHub.

1. **First things first:** Get familiar with the [LIME repository](https://github.com/marcotcr/lime) on GitHub. Please read the README: https://github.com/marcotcr/lime.
1. Get the tutorial notebook running on your computer. You find the notebook under assignments: https://github.com/FUB-HCC/hcds-winter-2020/tree/main/assignments/A5_Explanation. I added the `lime` package to `poetry`, so it should be enough to run `poetry install`.
1. Please step through the notebook and understand what is happening in each line. Please add markdown cells to your notebook to document your understanding of what is happening. You can also write down the question you have in mind, while stepping through the notebook or include links or references you used to get a deeper understanding of the notebook. (🔲 annotated notebook) **[2 points]** 🔴 🔴 
1. Get explanations for three different documents of the given [newsgroup dataset](https://scikit-learn.org/stable/datasets/#the-20-newsgroups-text-dataset) (currently document number 83 is used).  (🔲  plots) **[1 point]**🔴 
1. **Reflection**: Please answer the following question (🔲 two sentences per question ➡️ total ~250 words) **[3 points]** 🔴 🔴 🔴 
    1. Which documents did you choose?
    1. What did you learn about the model?
    1. How _well_ do you think the classifier works? Why?
    1. For what role(s) (from task 1) are LIME explanations useful? Why?
    1. How useful is LIME for a non-data-scientist (e.g. non-ml-experts or designer)? Why?
    1. What **question types** is LIME able to answer? Why?


_LINK to your annotated notebook here_

_1: ID and IMAGE of your LIME explanations_
_2: ID and IMAGE of your LIME explanations_
_3: ID and IMAGE of your LIME explanations_

### Optional Tasks
> ❗ The following tasks are **optional**. For the following tasks, please consider the frameworks: [alibi explain](https://github.com/SeldonIO/alibi), [lime](https://github.com/marcotcr/lime), and [interpretML](https://github.com/interpretml/interpret).
Please note: alibi explain and interpretML are libraries and include several local and global explanation methods, some we talked about in the lecture and some we did not. ❗

#### Task 3️⃣ &nbsp; Explanation methods for ORES (optional) [10 points]

**Goal:** 🥅 &nbsp; The goal of this task is to use a specific explanation method to explain your ORES model from `A4`.
**Hint:** This task is experimental and is targeted to students, who want to dig deeper into specific explanation methods from a more technical perspective.

1. Please choose ONE explanation method from alibi explain, lime, or interpretML. If you want to stick with LIME, then you can also look into the notebook by Adam Wight: https://github.com/adamwight/ores-lime.
    * Which method did you choose and why?
    * Please explain briefly what your method does.
    * Please describe if this method is model-agnostic or model-specific and if explanations are local or global.
1. Connect your ORES model with your chosen explanation method and provide a notebook with comments. **[8 points]**
1. **Reflection:** Please summarize what you did, how you did it, and what you have learned. (150 words) **[2 points]**

##### Deliverables
- [ ] Notebook with comments.
- [ ] Short written text with 150 words.
- [ ] Please include everything in your blog post.

#### Task 4️⃣ &nbsp; Design an Explanation Interface for ORES (optional) [10 points]
**Goal:** 🥅 &nbsp; The goal of this task is to get a deeper understanding of a specific explanation method and to prototype an explanation interface for your ORES model from the last assignment `A4`.
**Hint:** This task is experimental and is targeted to students, who want to prototype an explanation interface and to dig deeper into the design and HCI part of explanations.

1. Choose an explanation method from alibi explain, lime, or interpretML.
1. Choose **two roles** you want to design for. This relates the roles of task 1.
1. Create two explanation interfaces. As a prototyping tool, you could use [Sketch](https://www.sketch.com/), [Invision](https://www.invisionapp.com/), [Balsamic](https://balsamiq.com/wireframes), [figma](https://www.figma.com/prototyping/), or any other prototyping tool. You can also just use a pen & paper! **[7 points]**
    * What **specific question** do you want to answer?
    * What **question type** you are designing for?
1. Please provide **screenshots** of your two prototypes.
1. **Reflection:** Please summarize what you did, how those interfaces differ, and what you have learned. (150 words) **[3 points]**

##### Deliverables:
- [ ] Two screenshots
- [ ] Short written text with 150 words.
- [ ] Please include everything in your blog post.



#### Reflection
_your TEXT here_
