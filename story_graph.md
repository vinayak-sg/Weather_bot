digraph  {
0 [class="start active", fillcolor=green, fontsize=12, label=START, style=filled];
"-1" [class=end, fillcolor=red, fontsize=12, label=END, style=filled];
1 [class="", fontsize=12, label=utter_greet];
"-4" [class=ellipsis, label="..."];
3 [class=active, fontsize=12, label=action_weather];
4 [class=active, fontsize=12, label=utter_goodbye];
5 [class="intent dashed active", label="  ?  ", shape=rect];
6 [class=intent, fillcolor=lightblue, label=greet, shape=rect, style=filled];
7 [class="intent active", fillcolor=lightblue, label="weather in berlin", shape=rect, style=filled];
8 [class="intent active", fillcolor=lightblue, label="bye bye", shape=rect, style=filled];
0 -> "-1"  [class="", key=NONE, label=""];
0 -> 6  [class="", key=0];
0 -> 7  [class=active, key=0];
1 -> "-4"  [class="", key=NONE, label=""];
3 -> 8  [class=active, key=0];
4 -> 5  [class=active, key=NONE, label=""];
6 -> 1  [class="", key=0];
7 -> 3  [class=active, key=0];
8 -> 4  [class=active, key=0];
}
