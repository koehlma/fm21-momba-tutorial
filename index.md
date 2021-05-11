## FM21 Momba Tutorial


[Momba](https://momba.dev) is a Python framework for working with quantitative models centered around the [JANI model interchange format](https://jani-spec.org).

Dealing with quantitative models encompasses a variety of tasks which can be challenging from time to time.
Everything starts with the *construction* of a formal model or a family thereof.
Often a textual or other, more formal, description of the scenario to be modeled already exists, such as a rough sketch of the desired behavior or a circuit diagram.
Then, after a formal model has finally been conceived, one has to *validate* that the model actually adequately represents what should be modeled.
In this regard models are just like any other human artifact, inadequate initially but over time it gets better.
Only after confidence in the model has been established, one is able to harvest the benefits by handing over the model to *analysis* tools, e.g., a model checker.

In this tutorial, we will guide the participants through this process using a concrete example inspired by the [Racetrack benchmark](https://racetrack.perspicuous-computing.science/).
Participants will learn (1) how to leverage Momba's API to programmatically turn a domain-specific scenario description (e.g., a map of a game or a circuit diagram) into a quantitative model, (2) how to validate and test such models using Momba's explicit state space exploration engine by prototyping a tool for interactive model exploration and visualization, and (3) how to use the unified interfaces provided by Momba to invoke state-of-the-art tools for model analysis.

Over the past decade, Python has gained popularity especially in academia where the requirements for reproducibility are high.
Hence, in this tutoral, participants will also learn how to use Python and set up a project in a way enabling collaboration and easy packaging of reproducible artifacts.

We plan to run the tutorial as an interactive online event interleaving talks with hands-on sessions.
We will provide the participants with material on how to prepare their computer for the tutorial upfront.

The hands-on experience will be based on the example of a jump'n'run game where a player has to move from left to right at a constant speed while avoiding obstacles by moving up or down.
The actions of the player are subject to probabilistic noise, \ie, not every action has an effect and the player may continue moving straight instead of moving up or down.
The participants will construct a formal model based on a map of the game, write an interactive simulation and visualization based on the model using Momba's explicit state space exploration engine, and analyze the model with [The Modest Toolset](https://modestchecker.org) and [Storm](https://www.stormchecker.org/).
We provide the participants with a project skeleton for the example.
