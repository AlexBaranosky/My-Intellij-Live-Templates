These are the Intellij Live Templates I like to use to make developing in Java, Scala and Clojure more fluid.  Why spend your time/effort typing, when you could use it thinking about the problem at hand?

I've kept all my live templates to 2-3 chars for consciseness.

How to Use Them
===============

1. Open user.xml, copy out all of the <template> nodes, out of the <templateSet>

2. Go to ~/.IdeaC10/config/templates/user.xml (on Windows, the .Idea[xyz] folder is probably in your home directory, but I haven't checked.  Also, it will have a slightly different name depending on version number, or whether you are using Community edition or Ultimate edition.

3. To ~/.IdeaC10/config/templates/user.xml append my <template> nodea to your <templateSet> node, and save.

4. Enjoy the goodness.


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

fa

    (fact "$TITLE$"
      ($EXPR$) => $RESULT$)

tf

     (tabular
       (fact "$TITLE$"
         ($EXPR$) => $RESULT$)

       $TABLE$)

p

    (provided
      ($EXPR$) => $RESULT$)

Java Templates
==============
gw

     given($MOCK_OBJECT$.$METHOD$($ARGS$)).willReturn($RETURN_VALUE$);

sc

     public static class $CLASS_NAME$ {
         $CODE$
    }

mk

     mock($CLASS_NAME$.class);

el

     element("$NAME$", $BODY$)

tst

     @Test
     public void $NAME$() {
         $TEST_CODE$
     }

ae

     assertThat($ACTUAL$, equalTo($EXPECTED$));

ane

     assertThat($ACTUAL$, not(equalTo($EXPECTED$)));

an

     assertNull($ACTUAL$);

as

     assertThat($EXPR$, hasSize($EXPECTED_SIZE$));

Scala Templates
===============
tbl

    val testCases = new org.scalatest.prop.TableDrivenPropertyChecks.Table(
        ($TITLE_ROW$),
        ($ROW_1$),
        ($ROW_2$))

    forAll(testCases) { case ($TEST_CASE_DESTRUCTURING$) =>
        $TEST_EXPR$
    }

tst

    test("$TITLE$") {
        $TEST_CODE$
    }

sb

    should be ($EXPECTED$)

snb

     should not be ($EXPECTED$)
