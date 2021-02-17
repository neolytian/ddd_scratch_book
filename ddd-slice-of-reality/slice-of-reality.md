# Slicing the Reality

Slicing the reality in modelling comes from a discussion session I participated with [Mathias Verraes](https://verraes.net/) at the [DDD Europe 2021](https://dddeurope.com/). He formulated the idea of "Fractal inconsistencies". The idea is that each action or event creates physical imbalance which requires some action to be taken or event to happen. Based on the Event Storming we did as a modelling exercise we saw that Event Storming results can be broken down into different slices per persona. The hypothesis was, that each person has only a limited perception of the reality or of a process. So it is possible to model processes based on different personas and create better picture of the reality by putting the different slices of reality together.

## What is Domain Driven Design?

**[Domain Driven Design](https://en.wikipedia.org/wiki/Domain-driven_design)** is a discipline in software modelling. The term was invented by [Eric Evans](https://www.amazon.com/Domain-Driven-Design-Tackling-Complexity-Software/dp/0321125215/).

The concept of Domain Driven Design revolves around the idea that the language of the code should match the language of the business domain, the **[Ubiquitous Language](https://martinfowler.com/bliki/UbiquitousLanguage.html)**.
**[Bounded Context](https://en.wikipedia.org/wiki/Domain-driven_design#Bounded_context)** logically encloses a part of the business domain. This boundaries enables this sub domain to define its own ubiquitous language and behavior.

## Event Storming & Blink Modeling

![Event Storming Legend](.drawings/eventStormingLegend.png) //TODO: Fix Picture

[Event Storming](https://en.wikipedia.org/wiki/Event_storming) is workshop-based modelling method. The grammar of the Event Storming follows this order:

**TODO: Add Example for Event Storming**

- Event: An event capture a fact that happened. It is always written in past tense (e.g. Pasta cooked)
- Policy / Business Process: A policy is a business decision / rule.
- Command: A command expresses an intent. This intent is always written in present tense (e.g. cook pasta)
- Persona / Actor: The actor is the person who is executing the (parts of or the complete) business process
- Aggregate: An aggregate encloses the data (entities and value objects) and behavior of a logical unit within a process.

In the session with [Mathias Verraes](https://verraes.net/), he tends to use an additional symbol:

TODO: Add Screenshot of the Process Determination

- Process Determination: The Process Determination indicates if a process start or ends.

**[Blink Modelling](https://miro.com/app/board/o9J_lWERCMg=/)** is special form of Event Storming.
The rules are the following:

1. Every (decision path) has to be finished.
2. The Color Grammar has to be followed.
3. Every Stakeholder has to be reasonably happy.
4. Every hotspot must be addressed.


## What is a Persona?

As mentioned above a persona is an actor in a process. A persona can be seen as a stereotypical representation of a process participant. In a modelling or design workshop you define the attributes of such a persona: 

- First Name and Last Name
- Age
- Gender
- Day in the Life of the Persona
- Hobbies, Social Environments

## Slicing the reality per Persona

I know a long intro. Since we have now understood, what a event storming and blink modelling is and what a persona defines, let's bring it all together.

<------------>
Drawing of a process with several personas
<------------>

**First** you define your set of persona who are involved in the overall business domain. Do this with your group of domain experts at hand. You capture them in a [persona canvas](https://drawio-app.com/create-a-value-proposition-canvas-with-draw-io/).

**Second**, you perform an event modelling per persona. Invite at least one domain expert representing the persona.

**Third**, after you have performed the event modelling, you analyse the event storming for connection to the other process steps (events or command) in the other Event Storming Sessions. You need to identify process steps which influence the process of other personas (event, command, policies). These process steps are then the lead-out and lead-in to the other persona's reality.

**Fourth**, investigate within and across the modelled process if the parts of the process can be grouped logically into one bounded context revolving around the same (or same set) of aggregate(s).

## Conclusion

The "Slicing-of-Reality" Method give you a tool which enables you to wholistically model a process based on the different PoV of a personas. Hidden complexities and dependencies within the business process might become explicit across the different personas. You might be able to discover new interaction patterns between your personas by streamlining and simplifying your process.
