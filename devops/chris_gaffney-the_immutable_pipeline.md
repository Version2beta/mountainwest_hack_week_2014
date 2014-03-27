# The immutable pipeline

Chris Gaffney, Collective Idea, @gaffneyc

Dead Man's Snitch - monitoring tool for cron jobs deadmanssnitch.com

## Immutable

* Immutable object is an object whose state cannot be modified after it is created.
* Servers can be immutable in that, once they're configured and booted, we don't make changes again.

## Configurable

* Configure services on first boot

## Consistent

* Images and immutable services remain consistent

## Expendable

* Most immutable servers are expendable. Exceptions are database servers. Blow them away, recreate them.

## Pipeline

* Compile (an image) (speaker uses Packer)
* Test
* Deploy

Fuck, that kinda sucked. There's a lot more opportunity here.

