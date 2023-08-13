# Runelite Chat Filter RegEx
Regular expressions for the Runelite Chat Filter plugin to filter spam and things that annoy me.

This combines what I have found in a few Reddit posts as well as what I've personally added over time. Some entries are in a different format than what I use, but they work so I don't really see a need to fix it. This list will never be perfect, but it will remove the majority of spam/scam messages.

## To do
* Reduce redundancies

# How to use
1. Set "Filter type" to "Remove Message"
2. Check the box for "Strip accents"
3. Copy and paste the below text into the appropriate boxes. If you don't care about the "annoyances", don't copy that section.

### Filtered Names
```
(coin|royal|vegas|veg|raise|gamble|rng|roll|trusted|frost|dice|host) .{3,4}
.{3,4} (coin|royal|vegas|veg|raise|gamble|rng|roll|trusted|frost|dice|host).*
Casino
BET-
BET .+
```

### Filtered Regex
```
##Annoyances##
^.*Joel.*Skype.*
^.*mr br?e+a+s+t.*
^.*br?e+a+s+t burger.*
^.*just tried to do something very silly!
^.*(trump|biden) \d{2,5}.*
^.*just.*assume.*(my|his|her).*gender?.*
^.*identify as.*helicopter.*
^.*discord.*(\.|,).*gg.*

##Swapping##
^.*fat swap.*
swap.+rs3.+\(\)7.+d.?m.?m.+join.+cc
[<gt>\[]+ *(99 swap|trade rs|gamer swap|ac swap|eco swap|coswap) *[<lt>\]]
<gt> *(trade rs|gamer swap|ac swap) *<lt>
<gt> *eco *swap *<lt>
to swap your RS3
safe rs3 and 07 swap.*
lee swap

##Warnings##
^.*\[.+\] is a lurer using glitches to scam you out of( your)? items!* *$
^.*\[beware\] these players are (scam|lur)
^.*\[beware\] of the following pvp (scam|lur) 
^.*\[.+\] is a known (scamm|lur)er
^.*[\w -_]{1,12} is a (scamm|lur)er( beware,)? tr(ying|ies) to gain( ur)? trust w/ fake antiscam!
^.*scam+ers alert! "
^.*add '[\w\-_ ]+' *to ignore, (he will try to gain ur trust w/|tries gaining trust with) fake antiscam! *$
^.*beware (of )*fake antiscams, if it's too good to be true; then it is! *$
^.*lurers to ignore\:
^.*\].*are hacked accounts to scam!* *$
^.*do n\.?o\.?t search for (keyword )?giveaways on youtub
not safe on pvp.+you never get the sceptre
scammer on hacked account
^.*is a (well)?.*(known)? lurer.*
^Do not trust \[.*
^.*gpstall.*
^.*\[B.w.r.\].*f.th.s.*sc.mm.rs.*
^.*\[.+\].*ppl.*sc.m.*
^.*scam tactics are old.*
^.*plz+ help me report.*
^.*keep the reports coming.*
^.*this scammer.*using a fake.*bot
^\[.+\] is manipulating you to.*
^\[.+\] convinces you to help.*
^.*scammer:.*pretender.*
^.*fake anti-scam story.*


##Begging##
^.*(does )?any[ -]?(one|body)( (in )?here)? (have|got) *(a|some)?( full)? rune *(armou?r *)?(se?t)?( for me( to (have|keep))?)?\?* *$
^.*(take?|ac+ept)ing( al+)? (gift|donation|trade)s?( pl(ease|[sz]))? *$
^.*dance?ing (for|4) (money|coins|items|\d{1,4} *[kmb](il+)?)[!\.]* *$
^.*selling jokes?!* *$
^.*dancing for (free )?(money|items|gp|junk|stuff)!* *$
^.*take?ing a(ll|ny) (junk|item)
^.*clean out your banks! *$
^.*first to give me \d+m.*
^.*can anyone donate \d*.*
^.*someone (trade me|spare) \d+ *(m|k|b).*
looking for genuine people.*

##Scams##
^.*spending 2147m.*
^.*spending max cash.*
^.*show \d+ *[kmb](il+)? for (max cash|2[\.,]?147 *m|2([\.,]1)? *b)
^.*2(.1)?b for[ \?]*$
^.*show inv(en?tory)? for (\d{1,4}[bm]|max (cash|stack))
^.*(spending|offer for) (max cash|2[\.,]?147 *m|2([\.,]1)? *b) *\??
^.*do?ub+ling? (all )?(coin|gp|money|gold|item)[sz]? *!* *$
giving \d{1,3}( percent|%) of what you (show|trade)
^.*rewarding generosity!* *$
increasing banks by 10% 1 time only 1 trade
^.*trade?ing up .+
^.*doubling (money|g(old|p)).+\d{1,4} *[kmb](il+)? left
^.*buy(ing)? (g[hr]+azi|rap[ie]+r|t(wisted|[ -]?bow)|el+y|dwh).* (\d{3,4} *[kmb](il+)?|max (cash|stack|gp))
^.*(buy|sel+)ing (all )?burn(t|e?d) food
^.*(buy(ing)?|sell me( all)?) (sanguinesti staff|dragon hunter lance|kodai wand|ancestral set|arcane spirit shield|dragon hunter crossbow|dhcb|dragon claws|dragon warhammer|armadyl set and dhcb|armadyl set|scythe of vitur|inquisitor|ancient? hilt?|arcane and ancestral set) (\d+m.*|good offer!*|no joke.*)
^.*lo+l i pay \d+m for.*
^.*buying all valuable items.*
^.*t ?bow.*\?+ sell me for.*
^.*sell(s)? me all( your)? (bank|valuable items).*
^Doubling your money \d+m
^Who'll give me \d+m knowing.*
^.*Show me over \d+m.*
^.*(multiply|double|triple) your gold.*
^.*selly? my bank for \d+m

##Phishing and Services##
^.*crypto currency needs.*
next \d+ players get \d+ *[kmb](il+)?.+you[ -]*tube
.+chance.+win.+t([ -]?bow|wisted).+you[ -]*tube
^.*\(\)fuckm.*
fuck(\(\)|0|o) fuckm
^.*youtube.*to.*enter.*
^.*quitting,next 25 plyrs get
^.*quitting,\d{1,4}[bm] gp giveaway search youtube:-
r *s *m *a *l *l *s *\. *c *
next \d{1,3} players gets? \d{1,3}m.+search.+\w{3,4}\d{3,4}.+(facebook|youtube)
^.*huge \d{1,3}[mb] giveaway started!+ *$
^.*search ".+" on facebook *$
^.*\d{1,4}[mb] giveaway.+first come first serve! *$
^.*(((1 ?|fir)st|next) )?(one|player|person|user|account|guy|dude)? to show( me)? .+ (will )?(win|get|rec[ei]+ve?)s?
^.*watch the video follow the steps and trade me!
^.*visit rngbets\.net
 y[0o]u?tube *<gt> *[a-z]{3,4}\d{3,4} *$
s *e *l *l *r *s *0 *7
watch and win [a-z]{3,4}\d{3,4} ytbe *$
you,_,tube to win n0w *$
(win|give[ -]?away).+["']*[a-z]{3,4}\d{3,4}["']* [o0]n y[o0]u?,? ?tu?be *$
^.*(l|i)nfernos*cape.+(g+|c(o|0)).*
twitch.+giveaway.+drop part
mainrentals
raffles and giveaways
quitting giveaway
^*players.*search Youtube.*
Need a Infernal Cape?
^.*07.*drop party tonight.*
^.*g.*i.*v.*e.*a.*w.*a.*y.*tube.*
^.*cape.C0.*
^.*y0tube -.*
^.*y0u?tube.*
^.*(inferno|service).*c0m.*
^.*C *<> *M.*
^.*tube.*\D{3,4}\d{3,4}
^.*rsmarket.*
^.*runesh(o|0)p.*

##Gambling##
^.*(imposter|warning)+:.*(play fakes|fake host)+.*
^.*w-o-n \d+.*[kmb].+with a roll of
^.*\d+.*[kmb] paid out to .+ @ \d\d:\d\d:\d\d [ap]m *$
\| *\( *\d+ *k min(imum)? *\) *\|
\| (arena|duel|low|high|(royal )?slots|odd) \(![adlhsro]\)
\| legit dice games
was to busy trade declined \(\d/\d\)
roll of \(
 you löst with röll of
\| *5[45]x2 *\|
join.+cc.+legit.+dicing
 has ((won|lost) slots|been paid).+\[\d\d:\d\d:\d\d\] *$
over \d{1,3}.\d\d(b|t) paid
^.*automated host \|
^.*runebet \(\)
ubc bets.+win more
over.+paid ! \|
\|.+dice war.+\|
^.*massive payouts *\|
\| trusted & fun dicing
^casino located @
has (won|lost)( \d+[km]!?)? with a roll of
my m[iíl1]n[iíl1]m[uüú]m and max[iíl1]m[uüú]m bet [iíl1]s between
has received their winnin?gs of:
t bet on fakes! \|
 \|\| huge payouts!
rng \d{4,5} [0-2][0-9](:[0-5][0-9]){2} *$
^.*trade accepted for .+ amount: \d{1,4} *[kmb](il+)?
- \(trade to play\) - 
rolled a \[ \d{1,2} \] and 
 has (been paid the|traded) \[ \d{1,4}(\.\d+)? *[kmb](il+)? \]
 my m[iíl1]n[iíl1]m[uüú]m and max[iíl1]m[uüú]m is \[
\|\| huge payouts
^.*trade from .+: \d{1,4} *[kmb](il+)?
\| rng \d{4,5} [0-2][0-9](:[0-5][0-9]){2} *$
 wins! \d{1,4} *[kmb] *(il+)? with a \d{1,3} *$
 has received: \d{1,4} *[kmb](il+)? *$
 my bet (are|is) \d{1,4} *[kmb](il+)? coins\. *$
\[gembets\]
\| *\d{1,4} *[kmb](il+)? m[iíl1]n[iíl1]m[uüú]m *\|
^.*[\w\-_ ]+ lost :\( with a \d{1,3} *$
^.*[\w\-_ ]+ wins! \d{1,4} *[kmb](il+)? with a \d{1,3} *$
^.*[\w\-_ ]+ has received: \d{1,4} *[kmb](il+)? *$
^.*[\w\-_ ]+ my bet (are|is) \d{1,4} *[kmb](il+)?\+ coins\. *$
^.*the queue has \(\d{1,3}\) people\.( *\[\d{1,3}\] (win|loss) streak!)? *$
\| *55 *\+ wins! *\|
^.*congratulations to [\w\-_ ]+ on a win of \d{1,4} *[kmb](il+)?! *$
^.*(my m[iíl1]n[iíl1]m[uüú]m and maxim[uüú]m bet is|this machine only accepts coins\.) \(\d{1,4} *[kmb](il+)? to \d{1,4} *[kmb](il+)?\) coins\. try again\. *$
\| *\d{1,4} *[kmb](il+)? m[iíl1]n([iíl1]m[uüú]m)? *\|
^.*[\w\-_ ]+ has declined the trade\. *$
^.*trade accepted by [\w\-_ ]+: \d{1,4} *[kmb](il+)? *$
[\|l] *roll( over)? 5[45]\* *[\|l]
^.*bot still works while muted
^.*\([\w\-_ ]+\) has (been paid|cashed in)
^.*massive payouts!
you (have )?rolled a \(\d\d\)
^.*\*+ has won:
(won|lost) (with ?|roll ?){2} .?\d{1,3}
^.*roll 5\d\+
^.*hotroll:
\) roll \d\d *\+ \(
\(game: .+\) id: \d+ *$
has cashed in: *\d{1,4} *[kmb](il+)?
has run out of time. try again. *$
lost with a roll of \(\d+\) *$
lost fruit slots with \(.+\) *$
uidhosts\.net
has been paid *\d{1,4} *[kmb](il+)?! @
^.*hide your name from game results with \(!p\)rivate\. *$
^\[Private\] has.*
^.* has cashed in:
^.*D\u2014.*
^.*P\.A\.I\.D\.*
^.*P—A—I—D.*
Hide your name from game
^.*<\d+>.*Fròst.*
^.*bet mystery box is active!
^.*trading with.*current game:.*
^.*has Lost slots \(.*
^.*opened the mystery box and received a bonus \d.*
^.* has been paid:.*
^.*has paid.*\[\d+(m|k|b)\]
^.*(won|lost) \d+(m|k|b) with a roll.*
^.*winner.*\[\d+(m|k|b)\].*
^.*\[.*payouts?\].*
^.*Massive? Payouts.*
^.*Huge Winnings.*
^.*\[(lost|won)\].*
^.* \| trading:
^.*open dicing host.*
^.*\[high ?55\].*
^.*!v(erify)? automation
^.*this proves it'?s automated.*
^.*\[.*c.*r.*a.*w.*s.*\].*
^.*sad I got sniped on the other world.*
^.*runebets.*
^.*Automation \[.\].*
^.*trade requirement ready.*
^.*gamble now!.*
^.*\(!V\)
^.*5\dx2.*
^.*play responsibly.*limits.*
^.*id: *\d{3,}
^.*<\d+:\d\d>.*
^.*[("]coin fair[)"].*
^.*» *available «.*

##Unsorted##
