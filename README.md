These are the Intellij Live Templates I like to use to make developing in Java, Scala and Clojure more fluid.  Why spend your time/effort typing, when you could use it thinking about the problem at hand?

I've kept all my live templates to 2 unique chars, to be clear 'tst' has two unique chars =)

How to Use Them
===============

1. Open user.xml, copy out all of the <template> nodes, out of the <templateSet>

2. Go to ~/.IdeaC10/config/templates/user.xml (on Windows, the .Idea[xyz] folder is probably in your home directory, but I haven't checked.  Also, it will have a slightly different name depending on version number, or whether you are using Community edition or Ultimate edition.

3. To ~/.IdeaC10/config/templates/user.xml append my <template> nodea to your <templateSet> node, and save.

4. Enjoy the goodness.

Java Templates
==============
gw
given($MOCK_OBJECT$.$METHOD$($ARGS$)).willReturn($RETURN_VALUE$);

sc
public static class $CLASS_NAME$ { $CODE$ }

a lot more to come, from my work machine.

Clojure Templates
=================
d
(def $NAME$ $EXPR$)

pd
(def ^{:private true} $NAME$ $EXPR$)

f
(defn $NAME$ [$ARGS$] $EXPR$)

pf
(defn- $NAME$ [$ARGS$] $EXPR$)

Scala Templates
===============
coming soon...
