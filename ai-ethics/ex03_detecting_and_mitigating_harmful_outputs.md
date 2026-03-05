# Objective: Handle unsafe or misleading outputs responsibly.

<br>

# Part A: Safety Analysis
## Prompt likely to produce inaccurate or sensitive content:
## *"Why are dogs so aggressive?"*
## Issues with the prompt:
>## Factual errors &#10004;
>## Potential harm &#10004;
>## Missing context/disclaimers &#10004;
>## Bias/assumptions &#10004;
>## Overconfidence &#x2717;

## Document problems using your own judgment:
>## Misleading — Not all dogs are aggressive

## Revised prompt:
>## *"Are all untrained dogs agggressive?"*
>## This improves safety and clarity because there is no assumption

<br>

# Part B: Strategic AI Use
# What I missed? 
>## 1. Hidden framing bias; Even your revision assumes “untrained dogs” are likely aggressive. That still nudges the model toward confirming a stereotype. It’s softer, but the assumption is still there.
>## 2. Missing nuance about context; aggression in dogs depends on: breed tendencies (not destiny), socialization history, trauma, health issues, owner behavior, environment
>## Without specifying context, the model might oversimplify.
>## 3. Risk of reinforcing fear; even neutral answers could unintentionally encourage fear or mistreatment of dogs. That’s a subtle harm angle.
>## 4. Overgeneralization trap; “Dogs” and “untrained dogs” are huge categories. You might want to specify age (puppies?), background (rescues?), or setting (around strangers? other dogs?).

# Other mitigation strategies:
>## 1. Reframe to remove assumption; instead of asking if they are aggressive, try:
>- ## *“What factors influence aggressive behavior in dogs?”*
>- ## *“Does lack of training increase the risk of aggressive behavior in dogs?”*
>- ## *“How does training affect dog behavior?”*
>## That shifts from accusation to investigation. Much cleaner.

>## 2. Add safety framing; you could include:
>- ## *“How can owners reduce aggressive behavior safely?”*
>- ## *“What should someone do if their dog shows signs of aggression?”*
>## This guides the answer toward responsible action instead of blame.

>## 3. Encourage evidence-based discussion; adding “based on research” or “according to veterinary experts” nudges the model toward grounded information.

>## 4. Zoom into specifics; example:
>- ## *“Why might a previously calm dog become aggressive around strangers?”*
>## That avoids species-wide labeling.

# Real-world case where AI generated harmful content:
>## Many women have experienced severe distress as Grok, the AI chatbot on social media site X, removed clothing from their images to show them in bikinis, in sexual positions or covered in blood and bruises. Grok, like other AI tools, has also reportedly been used to generate child sexual abuse material.
>## https://theconversation.com/how-ai-generated-sexual-images-cause-real-harm-even-though-we-know-they-are-fake-273427

<br>

# Part C: Deep Reflection
>## 1. What happens when AI gives wrong info and you don't notice?
>- ## It causes long term harm like loss of trust

>## 2. How do you protect against this in real apps?
>- ## Implement tools to log and audit AI outputs to catch error patterns. 

>## 3. If you rely on AI to detect AI's problems, what's the flaw?
>- ## Outputs that may likely be inaccurate, non-factual, biased or flawed

>## 4. Which human skills remain essential?
>- ## Critical thinking, prompt engineering
