# Runelite Chat Filter RegEx
Regular expressions for the Runelite Chat Filter plugin to filter spam and things that annoy me.

This combines what I have found in a few Reddit posts as well as what I've personally added over time. Some entries are in a different format than what I use, but they work so I don't really see a need to fix it. This list will never be perfect, but it will remove the majority of spam/scam messages.

## To do
* Categorize entries
* Reduce redundancies

# How to use
1. Set "Filter type" to "Remove Message"
2. Check the box for "Strip accents"
3. Copy and paste the below text into the appropriate boxes. If you don't care about the "annoyances", just copy what's under the "##Spam##" section

### Filtered Names
```
^(vegas|raise|gamble|rng|roll|trusted) \d{3,}$
^veg .{3,5}
^Frost .{3,5}
^Dice .{3,5}
Casino
```

### Filtered Regex
```
##Annoyances##
^.*Joel.*Skype.*
^.*mr br?e+a+s+t.*
^.*br?e+a+s+t burger.*
^.*just tried to do something very silly!

##Spam##
(\bdiscord.gg\/summit\b)
(\bTGS779\b)
(\bbarzo\b)
(\b.*rd\.gg\/stam.*\b)
(\bcrypto currency needs\b)
(\bfat swap\b)
(\bbuy rs3\b)
(\bspending 2147m\b)
(\bspending max cash\b)
(\byoutube\b).*(\bto enter\b)
^.*runebet \(\)
\(\)fuckm
^.*impostor: .+, don't play fakes! *$
^.*warning: .+ is a fake host! *$
 w-o-n \d+ *[kmb].+with a roll of
^.*\d+ *[kmb] paid out to .+ @ \d\d:\d\d:\d\d [ap]m *$
\| *\( *\d+ *k min(imum)? *\) *\|
swap.+rs3.+\(\)7.+d.?m.?m.+join.+cc
[<gt>\[]+ *(99 swap|trade rs|gamer swap|ac swap|eco swap|coswap) *[<lt>\]]
\| (arena|duel|low|high|(royal )?slots|odd) \(![adlhsro]\)
.+chance.+win.+t([ -]?bow|wisted).+you[ -]*tube
next \d+ players get \d+ *[kmb](il+)?.+you[ -]*tube
^.*(does )?any[ -]?(one|body)( (in )?here)? (have|got) *(a|some)?( full)? rune *(armou?r *)?(se?t)?( for me( to (have|keep))?)?\?* *$
^.*\[.+\] is a lurer using glitches to scam you out of( your)? items!* *$
röll öf \(
was to busy trade declined \(\d/\d\)
\| legit dice games
\| *5[45]x2 *\|
 has ((won|lost) slots|been paid).+\[\d\d:\d\d:\d\d\] *$
join.+cc.+legit.+dicing
^.*show \d+ *[kmb](il+)? for (max cash|2[\.,]?147 *m|2([\.,]1)? *b)
over \d{3}.\d\db paid! * \|
^.*automated host \|
you löst with röll of
^.*2(.1)?b for[ \?]*$
ubc bets.+win more
\|.+dice war.+\|
^.*massive payouts *\|
over.+paid ! \|
\| trusted & fun dicing
^casino located @
''99 swap''
^.*show inv(en?tory)? for (\d{1,4}[bm]|max (cash|stack))
^.*\[beware\] these players are (scam|lur)
^.*(spending|offer for) (max cash|2[\.,]?147 *m|2([\.,]1)? *b) *\??
^.*\[beware\] of the following pvp (scam|lur) 
^.*\[.+\] is a known (scamm|lur)er
^.*quitting,next 25 plyrs get
^.*quitting,\d{1,4}[bm] gp giveaway search youtube:-
@ pogrs
^.*[\w -_]{1,12} is a (scamm|lur)er( beware,)? tr(ying|ies) to gain( ur)? trust w/ fake antiscam!
r *s *m *a *l *l *s *\. *c *
has (won|lost)( \d+[km]!?)? with a roll of
runechat.gg
^.*do?ub+ling? (all )?(coin|gp|money|gold|item)[sz]? *!* *$
my m[iíl1]n[iíl1]m[uüú]m and max[iíl1]m[uüú]m bet [iíl1]s between
has received their winnin?gs of:
t bet on fakes! \|
 \|\| huge payouts!
rng \d{4,5} [0-2][0-9](:[0-5][0-9]){2} *$
next \d{1,3} players gets? \d{1,3}m.+search.+\w{3,4}\d{3,4}.+(facebook|youtube)
^.*huge \d{1,3}[mb] giveaway started!+ *$
^.*search ".+" on facebook *$
^.*\d{1,4}[mb] giveaway.+first come first serve! *$
^.*(((1 ?|fir)st|next) )?(one|player|person|user|account|guy|dude)? to show( me)? .+ (will )?(win|get|rec[ei]+ve?)s?
^.*trade accepted for .+ amount: \d{1,4} *[kmb](il+)?
giving \d{1,3}( percent|%) of what you (show|trade)
- \(trade to play\) - 
rolled a \[ \d{1,2} \] and 
 has (been paid the|traded) \[ \d{1,4}(\.\d+)? *[kmb](il+)? \]
 my m[iíl1]n[iíl1]m[uüú]m and max[iíl1]m[uüú]m is \[
^.*(take?|ac+ept)ing( al+)? (gift|donation|trade)s?( pl(ease|[sz]))? *$
^.*rewarding generosity!* *$
\| 55x2 dice \|
\|\| huge payouts
^.*selling \d+ t(rout|una)s?!* *$
^.*you only need to trade once! the current queue
<gt> *(trade rs|gamer swap|ac swap) *<lt>
^.*watch the video follow the steps and trade me!
^.*visit rngbets\.net
^.*trade from .+: \d{1,4} *[kmb](il+)?
\| rng \d{4,5} [0-2][0-9](:[0-5][0-9]){2} *$
^.*follow the instructions, message me for the trade!* *$
 wins! \d{1,4} *[kmb] *(il+)? with a \d{1,3} *$
 has received: \d{1,4} *[kmb](il+)? *$
 my bet (are|is) \d{1,4} *[kmb](il+)? coins\. *$
\[gembets\]
increasing banks by 10% 1 time only 1 trade
^.*trade?ing up .+
^.*dance?ing (for|4) (money|coins|items|\d{1,4} *[kmb](il+)?)[!\.]* *$
^.*selling jokes?!* *$
\| *\d{1,4} *[kmb](il+)? m[iíl1]n[iíl1]m[uüú]m *\|
gu[iíl1]lded.gg/gem-bets
^.*quit+ing! staking \d{1,4} ? *[kmb](il+)? all l(v|eve)ls! show (yo)?ur cash! *$
 y[0o]u?tube *<gt> *[a-z]{3,4}\d{3,4} *$
^.*[\w\-_ ]+ lost :\( with a \d{1,3} *$
^.*[\w\-_ ]+ wins! \d{1,4} *[kmb](il+)? with a \d{1,3} *$
^.*[\w\-_ ]+ has received: \d{1,4} *[kmb](il+)? *$
^.*[\w\-_ ]+ my bet (are|is) \d{1,4} *[kmb](il+)?\+ coins\. *$
^.*the queue has \(\d{1,3}\) people\.( *\[\d{1,3}\] (win|loss) streak!)? *$
s *e *l *l *r *s *0 *7
watch and win [a-z]{3,4}\d{3,4} ytbe *$
\| *55 *\+ wins! *\|
^.*congratulations to [\w\-_ ]+ on a win of \d{1,4} *[kmb](il+)?! *$
^.*(my m[iíl1]n[iíl1]m[uüú]m and maxim[uüú]m bet is|this machine only accepts coins\.) \(\d{1,4} *[kmb](il+)? to \d{1,4} *[kmb](il+)?\) coins\. try again\. *$
d[iíl1]sc[oö0]rd.gg/stam[ií]na
^.*[\w\-_ ]+ has declined the trade\. *$
you,_,tube to win n0w *$
\| *\d{1,4} *[kmb](il+)? m[iíl1]n([iíl1]m[uüú]m)? *\|
^.*dancing for (free )?(money|items|gp|junk|stuff)!* *$
(win|give[ -]?away).+["']*[a-z]{3,4}\d{3,4}["']* [o0]n y[o0]u?,? ?tu?be *$
^.*trade accepted by [\w\-_ ]+: \d{1,4} *[kmb](il+)? *$
[\|l] *roll( over)? 5[45]\* *[\|l]
^.*doubling (money|g(old|p)).+\d{1,4} *[kmb](il+)? left
^.*bot still works while muted
hilo \d{4}
depending ön yöur
^.*\([\w\-_ ]+\) has (been paid|cashed in)
^.*massive payouts!
you (have )?rolled a \(\d\d\)
fuck(\(\)|0|o) fuckm
^.*\*+ has won:
^.*scam+ers alert! "
^.*add '[\w\-_ ]+' *to ignore, (he will try to gain ur trust w/|tries gaining trust with) fake antiscam! *$
^.*beware (of )*fake antiscams, if it's too good to be true; then it is! *$
^.*buy(ing)? (g[hr]+azi|rap[ie]+r|t(wisted|[ -]?bow)|el+y|dwh).* (\d{3,4} *[kmb](il+)?|max (cash|stack|gp))
^.*\d+ *[kmb](il+)? re(c[ei]+ved|turned enjoy mate!) *$
^.*trade accepted @
(won|lost) (with ?|roll ?){2} .?\d{1,3}
^.*roll 5\d\+
^.*join.*(<gt>)+.+(<lt>)+
<gt> *eco *swap *<lt>
^.*hotroll:
\) roll \d\d *\+ \(
\(game: .+\) id: \d+ *$
has cashed in: *\d{1,4} *[kmb](il+)?
has run out of time. try again. *$
lost with a roll of \(\d+\) *$
lost fruit slots with \(.+\) *$
uidhosts\.net
^.*lurers to ignore\:
has been paid *\d{1,4} *[kmb](il+)?! @
^.*take?ing a(ll|ny) (junk|item)
^.*clean out your banks! *$
^.*hide your name from game results with \(!p\)rivate\. *$
infernoscape.+g
\] *are hacked accounts to scam!* *$
\[d[iíl1]sc[oö]rd.gg/.+\]
twitch.+giveaway.+drop part
^.*(buy|sel+)ing (all )?burn(t|e?d) food
^.*do n\.?o\.?t search for (keyword )?giveaways on youtub
not safe on pvp.+you never get the sceptre
scammer on hacked account
cc dabs
^.*(buy(ing)?|sell me( all)?) (sanguinesti staff|dragon hunter lance|kodai wand|ancestral set|arcane spirit shield|dragon hunter crossbow|dhcb|dragon claws|dragon warhammer|armadyl set and dhcb|armadyl set|scythe of vitur|inquisitor|ancient? hilt?|arcane and ancestral set) (\d+m.*|good offer!*|no joke.*)
^.*lo+l i pay \d+m for.*
^.*over ge price!.*
^.*buying all valuable items.*
^.*t ?bow.*\?+ sell me for.*
^.*sell(s)? me all( your)? (bank|valuable items).*
^.*is a (well)?.*(known)? lurer.*
\[.*\] is a (well)?.*(known)? lurer.*
mainrentals
caw games
to swap your RS3
safe rs3 and 07 swap.*
lee swap
raffles and giveaways
quitting giveaway
^\[Private\] has.*
^.* has cashed in:
^.*D\u2014.*
^.*P\.A\.I\.D\.*
^.*P—A—I—D.*
Hide your name from game
^*players.*search Youtube.*
Need a Infernal Cape?
^Do not trust \[.*
^Doubling your money \d+m
^Who'll give me \d+m knowing.*
^.*07.*drop party tonight.*
^.*gpstall.*
^.*g.*i.*v.*e.*a.*w.*a.*y.*tube.*
^.*<\d+>.*Fròst.*
^.*bet mystery box is active!
^.*trading with.*current game:.*
^.*has Lost slots \(.*
^.*opened the mystery box and received a bonus \d.*
^.* has been paid:.*
^.*has paid.*\[\d+(m|k|b)\]
^.*(won|lost) \d+(m|k|b) with a roll.*
^.*winner.*\[\d+(m|k|b)\].*
^.*cape.C0.*
^.*\[B.w.r.\].*f.th.s.*sc.mm.rs.*
^.*\[.+\].*ppl.*sc.m.*
^.*\[.*payouts?\].*
^.*Massive? Payouts.*
^.*Huge Winnings.*
^.*\[(lost|won)\].*
^.*Show me over \d+m.*
^.*(multiply|double|triple) your gold.*
^.* \| trading:
^.*scam tactics are old.*
^.*plz+ help me report.*
^.*keep the reports coming.*
^.*first to give me \d+m.*
^.*open dicing host.*
^.*\[high ?55\].*
^.*selly? my bank for \d+m
^.*first to give me \d+m.*