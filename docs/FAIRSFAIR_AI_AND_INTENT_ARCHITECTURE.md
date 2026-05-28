# FairsFair AI, Voice & Intent Architecture

## Core Principle

Future AI and voice systems across the FairsFair ecosystem must operate as:
- intent suggestion systems
- workflow assistance systems
- structured action generators

They must NOT directly mutate application state or bypass core business logic.

## Architectural Rule

Voice and AI systems should never directly write persistent data.

```text
Speech/Text
    ↓
Intent Parser
    ↓
Structured Proposed Action
    ↓
Preview + Forecast Impact
    ↓
Explicit User Confirmation
    ↓
Persist + Recalculate
```

## Structured Intent Direction

Future interfaces should converge on a shared action architecture.

Example:

```js
{
  intent: 'create_transaction',
  amount: 12.40,
  merchant: 'Tesco',
  category: 'Groceries',
  account: 'Monzo'
}
```

## Explicit Confirmation Requirement

Voice-entered or AI-generated actions must require explicit user confirmation before persistence.

## FairsFair Money Direction

Potential future workflows:
- conversational Safe To Spend queries
- forecast simulation conversations
- voice-assisted transaction capture
- AI-assisted categorisation

## FairsFair Petcare Direction

Potential future workflows:
- voice-to-text booking searches
- voice-assisted coordination
- hands-busy workflows
- quick accept/reject booking flows
- AI summarisation of spoken instructions
- voice-triggered WhatsApp/SMS coordination

## Product Philosophy

Across the ecosystem:
- useful when needed
- invisible when not
- reduce cognitive load
- calm operational assistance
- continuity over addiction
- AI assists rather than replaces humans
