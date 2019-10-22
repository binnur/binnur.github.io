---
layout: post
date: 2019-09-24 10:33:45
title: "Why Building ML/AI Powered Products Hard?"
categories: ml-ai product-management
author_name : binnur
author_url : /author/binnur
author_avatar: binnur
show_avatar : true
read_time : 7
feature_image: post-droplets
show_related_posts: false
square_related: recommend-droplets
---
Full disclosure: I am not a ML/AI practitioner. However, I have worked on ML
products and have first hand experience on how challenging they can be for
organizations from product design and development to product and project
management. So, these articles are driven by my curiosity and reflect my
research and takeaways on how to tackle the process of building ML/AI powered
products that delight, and ensures there is a strong foundation to build from for
the organization.

Lets start with the definitions. For the purpose of this article, I will mainly
use/refer to ML and ML systems, however the concepts would also apply to AI.
* ML or Machine Learning is the use of computer and statistical algorithms to
  learn from data to detect patterns and make predictions.
* AI or Artificial Intelligence is the broader science of getting computers to
  act intelligently without being explicitly programmed.

For more on this topic, check out [Machine Learning vs. AI, Important Differences
Between Them](https://medium.com/datadriveninvestor/differences-between-ai-and-machine-learning-and-why-it-matters-1255b182fc6).

The rest of this article highlights different aspects of ML products that can make
them challenging for organizations.

* Also checkout Domino Data Science Field Note from [Machine Learning Projects are Hard: Shifting from a Deterministic Process to
  a Probabilistic One by Pete Skomoroch](https://blog.dominodatalab.com/machine-learning-product-management-lessons-learned/)

## Hard to tell, but ML is young
Given all the excitement around self-driving cars, voice-activated assistants,
and a world riddled with deepfakes, it is hard to believe these advancements are
only a couple of decades old. True, the ideas behind machine learning have a
long history, formalized in 1950 when Alan Turing asked the question *"Can
machines think?"*. However, with lack of visible progress, the mid-1970s were the
start of the *AI winters*, and it was in the 1990s when the field shifted to
data-driven approaches, combining statistics and computer science, where rapid
progress started. However, we are still learning what it takes to incorporate ML
into product development processes and how best to manage its lifecycle.

Software similarly had its own challenges as the cost of building software
skyrocketed, with 1965-1985 marking the period of *software crisis*. The
foundation of the term *Software Engineering* occurred in 1968/1969, when
conferences were held to improve software development processes and tooling.
As the speed of new product introductions accelerated, so did the increased
focus on modern application development with better tooling and methodologies.

For more historical highlights, checkout:
* [Aneri Sheth and History of Machine
  Learning](https://medium.com/bloombench/history-of-machine-learning-7c9dc67857a5)
* [A History of Machine
  Learning](https://cloud.withgoogle.com/build/data-analytics/explore-history-machine-learning/)
* [Wikipedia: History of Software Engineering](https://en.wikipedia.org/wiki/History_of_software_engineering)


## The true nature of ML is stochastic
While software is deterministic, ML is stochastic -- it is hard to
predict how a given dataset and model will respond in real life. This
nondeterministic nature makes it difficult when it comes to product and project
planning and management.

From the **product perspective**, uncertainty associated with ML development
challenges roadmaps and roadmap planning, progress and status communication to
stakeholders, and in managing expectations internally and externally. As data is
critical for developing ML capability, establishing a clear data-acquisition
strategy, and building a system that can learn as it gathers more data is an
iterative process that requires ongoing focus.

From the **project management** perspective, experimental and iterative nature of
ML lifecycle likely will not fit within a scrum methodology -- from personal
experience, kanban was a better framework. And, as one can spend forever on data
cleanup, feature engineering, and model development, timeboxing the activities
was critical. However, the ML development lifecycle is more complex than just
project management.


## The ML development lifecycle is iterative, production readiness is hard
ML projects are highly iterative and experimental. I found the experience
similar to working with designers but with more math. The end goal of the project
is to power your product with ML capabilities, and not just build a model.

> *"If you don't know where you are going, every road will get you nowhere."*
> --Henry Kissinger

The process starts with a clear articulation of the problem. As the project
progresses, assumptions will get validated and as new information is learned, the
project likely pivots. You may also have multiple experiment tracks running with
different datasets, features, models, and evaluation metrics. This exploration
process and the number of dimensions tested can get complex, fast -- this is why
it is important to have a clear vision of the goal post and a workflow that can
help manage the different inputs. And of course, all the changes will need to
be fed back to the project and product plan.

Ultimately, the goal is to get the ML model into production serving predictions.
While we had decades of experience fine tuning software development
pipelines, we are still figuring out ML workflows. Needless to say, many
startups are working to solve this problem. Challenges include, but are not
limited to:

* Managing and versioning the software stack, code and data with experiments for repeatability and reproducibility,
* Easy access to code and data for collaboration,
* Data policy and enforcement,
* Production deployment with monitorability for quality assurance,
* Model evaluation for explainability, fairness, bias, and ethics.


Good reads on the topic:
* [Machine Learning Yearning: Technical Strategy for AI Engineers, In the Era of
  Deep Learning by Andrew Ng](https://www.deeplearning.ai/machine-learning-yearning/)
* [Machine Learning: The High Interest Credit Card of Technical Debt](https://ai.google/research/pubs/pub43146)
* [The ML Test Score: A Rubric for ML Production Readiness and Technical Debt Reduction](https://ai.google/research/pubs/pub46555)


## ML is a product design problem
As impressive as the possibilities may be, ML projects ultimately need to meet
a customer or a business need. This takes us back to the importance of framing
the problem to ensure success of ML projects.

As there is *more than one way to skin a cat*, there is more than one way to
achieve the goal. As a product manager and design team, it is important to
understand both the desired and acceptable user experiences as part of this
problem framing. This is especially critical for objective evaluation of the ML
system for launch.

* ML output is a prediction, it is not 100% accurate. Customer trust is critical
  in building long lasting businesses. How will your users respond
  to the prediction, and how will the prediction be explained? Systems that
  explain how they work are better perceived by users as they support trust
  building.
* How about errors in prediction? Based on your application, what is the risk of
  giving wrong answers? And, how do you balance between the two? I remember the
  day I broke Netflix's movie recommendation. After rating 200+ movies, I
  received only 7 movie recommendations and I didn't like any of them...
* Given those insights, what are the potential user interactions and design
  approaches? And from that, what are the data dependencies and do they meet the
  level of needed data quality and freedom from biases? Once in production, what
  are your base performance metrics and how do you detect when models go stale
  and trigger a retraining cycle? If you you lack needed data, how do you handle
  the cold start problem?
* How would these desired experiences impact the rest of the development
  pipeline, such as the way search terms are indexed in the backend? Is this a
  batched/offline or real-time experience? How are the learnings fed back to the
  model and how often?
* Knowing the capabilities of ML is important, but knowing the capabilities of
  your organization is more so. While it is important to understand and identify
  high value applications for ML, and to differentiate between easy, hard, and
  impossible ML problems, it is more important to recognize that an effort vs.
  value judgement will need to take place. How much effort will result in what
  percent of product improvement?


Good reads on the topic:
* [Rules of Machine Learning: Best Practices for ML Engineering](https://developers.google.com/machine-learning/guides/rules-of-ml/)
* [Human-Centered Machine
Learning](https://medium.com/google-design/human-centered-machine-learning-a770d10562cd)
highlights 7 steps to stay focused on the user while designing with ML.


## ML is an organizational problem
As with any project, you need the right team to be successful. ML adds
new roles the organization with a team skilled in both Data Science and
Engineering to develop and maintain ML pipelines from data ingestion to
training, deployment, and insight extraction.

However, regardless of the team, if the organizational culture does not have a
culture of *data* literacy and a recognition of *experimentation*, getting to
the finish line is that much more difficult.

* ML products are about data, does the leadership prioritize and invest in data
  from its collection to insight generation?
* Data literacy impacts every part of the organization. How is the team learning
  and improving their data know-how to understand as well as derive insights?
* How well the team *knows its data* is correlated to how creative and purposeful
  the team can be at building powerful ML powered applications. Where is the data,
  how accessible is it, and how is its quality maintained/improved?
* Collecting and displaying data is one thing, but is the team encouraged to ask
  *'so what?'* questions for actionable insights?


## Change is the only constant in ML systems
ML applications are nondeterministic. An ML system learns from training data, but
data in the external world is not static. It changes as the users' usage
behaviors evolve. As a result, an ML system's prediction accuracy changes.
However, even the smallest change can have unintended consequences, such as
refactoring of labels or inputs.

Given that change is the only constant in ML systems, establishing baselines,
monitoring performance, and continuously evaluating system results for accuracy and
fairness is a must. It is a good practice to expect that your ML powered
application will fail, so brainstorm from users' perspective to identify graceful
ways to handle a wide range of failures.


## And, ML systems fail in unexpected ways
The Internet is full of stories on badly behaving ML/AI systems. This has given
rise to a focus on ethical AI design and guidelines, such with
[EU's Ethic Guidelines for Trustworthy AI](
    https://ec.europa.eu/futurium/en/ai-alliance-consultation/guidelines).
While I love the increased focus on human-centered and trustworthy AI, our ability
to objectively assess and evaluate these requirements will ensure its successful
execution. With that said, I am glad we are thinking and talking about it!
