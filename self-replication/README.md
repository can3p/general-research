# Self-replicating machines

Let's imagine we want to setup a colony on a distant planet or deep under the
surface or any other harsh conditions. One way to do it is to send all equipment
there and build it. The drawback is that assembled equipment and (especially)
people is very fragile and may not survive till the moment we finish with
the construction. Or, after the arrival it can appear that conditions in
the destination are much worse or just very different from initial expectations.
Say, we expected rock but got a sand-like structure instead or all water appeared
to be impossible to drink for whatever reason.

Wouldn't it be great to let machines do all the work? Let's look at this idea
in a little bit more detail. How many machines we would need? Several types,
most probably: lift parts, cut them, bolt them together, do reconnaissance or
any others, and maybe many different parts to assemble housing, infrastructure etc.

Any complex parts can be divided into simpler and smaller once as well as
most of machines. If we take it to extreem, we need only one machine at the beginning
with access to a big inventory of parts, the more generic the better. We can even
for an "egg" with single machine surrounded and shielded by equipment.

All machine knows is how to assemble it's own copy and few other types of machines.
If we unwrap this recursively while adopting to local conditions on every step
we can get to a very tailor-made version of settlement in the end.

Since it's sounds very complex, let's reduce this idea to one machine and one part
which is the same kind of machine, only turned off, and without initial program.

How can the program look like?

1. Search for new part
2. Flash the source of the program
3. Turn on
4. Repeat

After few iterations we can have all details turned on.

What can be the next step?

Let's say that every operation takes time and flashing and turning on cannot be
operated on the same machine except first one.

What should first machine do? Something like that

1. Check if there are other machines running.
2. If so, search and flash more parts.
3. If not, take first part, flash it with program 2 and enable it.

What's program 2?

1. Search for new unflashed part.
2. If non left, stand by
3. 50/50 chance of flashing it with turning on/flashing functionality,
4. Repeat.

What's program 3?

1. Search for new flashed part
2. If non left, stand by
3. Turn it on
4. Repeat

Next step can be about having resources of two types, one of which whould be produced
by yet another machine, that has to be assembled, and make machines assembled from
several parts

After this we can add durability for items meaning that some parts can break; in this
case machine should be fixed/disentangled into spare parts for others.
