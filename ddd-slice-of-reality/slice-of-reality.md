# Slicing the Reality

Slicing the reality in modelling comes from a discussion session I participated with [Mathias Verraes](https://verraes.net/) at the [DDD Europe 2021](https://dddeurope.com/). He formulated the idea of "Fractal inconsistencies". The idea is that each action or event creates physical imbalance which requires some action to be taken or event to happen. Based on the Event Storming we did as a modelling exercise we saw that Event Storming results can be broken down into different slices per persona. The hypothesis was, that each person has only a limited perception of the reality or of a process. So it is possible to model processes based on different personas and create better picture of the reality by putting the different slices of reality together.

## What is Domain Driven Design?

**[Domain Driven Design](https://en.wikipedia.org/wiki/Domain-driven_design)** is a discipline in software modelling. The term was invented by [Eric Evans](https://www.amazon.com/Domain-Driven-Design-Tackling-Complexity-Software/dp/0321125215/).

The concept of Domain Driven Design revolves around the idea that the language of the code should match the language of the business domain, the **[Ubiquitous Language](https://martinfowler.com/bliki/UbiquitousLanguage.html)**.
**[Bounded Context](https://en.wikipedia.org/wiki/Domain-driven_design#Bounded_context)** logically encloses a part of the business domain. This boundaries enables this sub domain to define its own ubiquitous language and behavior.

## Event Storming & Blink Modeling

[Event Storming](https://en.wikipedia.org/wiki/Event_storming) is workshop-based modelling method. The grammar of the Event Storming follows this order:

![Event Storming Legend](.drawings/eventStormingLegend.png)

- Event: An event capture a fact that happened. It is always written in past tense (e.g. Pasta cooked)
- Policy / Business Process: A policy is a business decision / rule.
- Command: A command expresses an intent. This intent is always written in present tense (e.g. cook pasta)
- Persona / Actor: The actor is the person who is executing the (parts of or the complete) business process
- Aggregate: An aggregate encloses the data (entities and value objects) and behavior of a logical unit within a process.
- Process Determination: The Process Determination indicates if a process start or ends.


Blink Modelling is special form of Event Storming.


## What is a Persona?

 
## Slicing the reality per Persona
