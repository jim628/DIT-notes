#ss-Information 
	[eclass](https://eclass.uoa.gr/courses/DI724/)
		Υπάρχουν Χειρόγραφες σημειώσεις
	Θα διατίθενται μαγνητοσκοπημένες οι διαλέξεις
	Βαθμός 100% Γραπτό

# δύναμη -----> Όχημα -----> Μετατόπιση
[[Signals and Systems Lecture 1.pdf#page=1&selection=8,0,117,4|Signals and Systems Lecture 1, page 1]]
δηλ. Θεωρώντας ένα σύστημα S θα λέμε: $$x(t) \rightarrow S(.) \rightarrow y(t)$$
- $x(t),\ y(t)$:  συναρτήσεις του t :: Σήματα
- $S$ : τελεστή / μετασχηματισμό :: Σύστημα
Δηλαδή: $$ y(t) = S(\underbrace{x(t)}_{ανεξάρτητη\ μεταβλητή}) $$
Έχουμε μία είσοδο x η οποία μετασήματίζεται σε μία έξοδο $y = S(x)$.

# Απόκριση Σηστήματος
[[Signals and Systems Lecture 1.pdf#page=2&selection=8,0,55,3|Signals and Systems Lecture 1, page 2]]
- Γνωρίζουμε το $x$
- Γνωρίζουμε το $S$
Υπολογίζουμε την απόκριση y

# Εκμάθηση Συστήματος
[[Signals and Systems Lecture 1.pdf#page=2&selection=57,0,105,6|Signals and Systems Lecture 1, page 2]]
- Γνωρίζουμε το $x$
- Γνωρίζουμε το $y$
Βρίσουμε ένα σύστημα S ώστε $y = S(x)$

# Έλεγχος Ανάδρασης (feedback)
[[Signals and Systems Lecture 1.pdf#page=2&selection=107,0,124,9|Signals and Systems Lecture 1, page 2]]
Βλέπουμε την έξοδο του συστήματος και την χρησιμοποιούμε (με έξηπνκ τρόπο) ώστε να διορώσουμε την είσοδο.
Θεωρούμε ένα σήμα αναφοράς r(t) όπου έπειτα διορθώνουμε:

r(t) --> \[ ανατροφοδότηση ] x(t) --> S(.) --> y(t) -> έλεγχοε >> ανατροφοδότηση

# Επεξεργασία Σήματος x(.)
[[Signals and Systems Lecture 1.pdf#page=3&selection=2,0,48,15|Signals and Systems Lecture 1, page 3]]
Θα χρησιμοιποιούμε διάφορους μετασχηματισμούς επί μίας εισόδου $x$.

# Βασικά Σήματα
[[Signals and Systems Lecture 1.pdf#page=4&selection=0,0,111,9|Signals and Systems Lecture 1, page 4]]
- Μοναδιαία βηματική συνάρτηση:
$$ u(t) = \begin{cases} 1 && t > 0 \\ 0&& t < 0 \end{cases}$$
- Κρουστική συνάρτηση Dirac
$$ δ(t) = \begin{cases} 0 && t \neq 0 \\ +\infty&& t = 0 \end{cases} \ \Rightarrow \int_{-\infty}^{+\infty}dxδ(x)=1$$
- Περιοδικές συναρτήσεις / σήματα:
$$ x(t) = x(t + kT),\ \forall k \in{Z} $$
$$ \sin(\underbrace{\omega t}_{\omega = \frac{2\pi}{T}} + \phi) $$
# Κατηγορίες Σημάτων
[[Signals and Systems Lecture 1.pdf#page=5&selection=0,1,4,9|Signals and Systems Lecture 1, page 5]]

## Συνεχούς Χρόνου - Αναλογικά
- Όταν ένα σήμα $x(t)$ ορίζεται για κάθε $t \in R$ ονομάζονται ***συνεχούς χρόνου***
- Όταν επίσης $x(t) \in R$ ονομάζεται ***αναλογικό***
[[Signals and Systems Lecture 1.pdf#page=5&selection=6,0,37,6|Signals and Systems Lecture 1, page 5]]

## Διακριτού Χρόνου - Ψηφιακά
- Όταν ένα σήμα $x(n)$ ορίζεται για κάθε $n \in N$ τότε ονομάζεται ***διακριτού χρόνου***
- Όταν επίσης $x(n) \in N$ ονομάζεται ***ψηφιακό***
[[Signals and Systems Lecture 1.pdf#page=5&selection=50,1,127,6|Signals and Systems Lecture 1, page 5]]

> [!Παράδειγμα Ψηφιακόυ Σήματος]
> Ένα παράδειγμα ψηφικού σήματος είναι μία οθώνη με pixel $n, m \in N$ και δίνουν ένα σήμα $x(n, m) \in N$ 

## Αιτιατά vs. μη αιτιατά σήματα
$αιτιατό \Leftrightarrow x(t) = 0, \forall t<0$ 
[[Signals and Systems Lecture 1.pdf#page=6&selection=0,0,37,6|Signals and Systems Lecture 1, page 6]]

## Ένεργιας vs. ισχύος:
### Ενεργιάς: 
Για να ένα σήμα $x(t)$ η ενέργιά του είναι:$$ E_x = \int_{-\infty}^{+\infty}|x(t)|^2dt $$
Για να είναι *ενέργιας* θα πρέπει: $0 <E_x <\infty$
### Ισχύος: 
Για να ένα σήμα $x(t)$ η ισχυής του είναι:$$ P_x = \lim_{T\rightarrow\infty}\frac{1}{2T}\int_{-T}^{+T}|x(t)|^2dt $$
Αυτό θα είναι σήμα ισχύως αν: $0<P_x<\infty$
[[Signals and Systems Lecture 1.pdf#page=6&selection=40,0,123,5|Signals and Systems Lecture 1, page 6]]
# Παράδειγμα
[[Signals and Systems Lecture 1.pdf#page=7&selection=0,0,148,10|Signals and Systems Lecture 1, page 7]]
Είναι το παρακάτω σήμα x σήμα ενέργιας.
$$x(t) = e^{-at}u(t), a>0$$
Υπολογίζουμε την ενέργια:
$$ E_x = \int_{-\infty}^{+\infty}|x(t)|^2dt = \int_{-\infty}^{+\infty}e^{-2at}u^2(t)dt = \int_{0}^{+\infty}e^{-2at}dt = \frac{1}{2a} >0$$
Άρα είναι σήμα ενέργιας.

Ομοίως να λύσετε τα:
- $x(t) = tu(t)$

# Κατηγορίες Συστημάτων
[[Signals and Systems Lecture 1.pdf#page=8&selection=0,2,0,3|Signals and Systems Lecture 1, page 8]]
## Δυναμικά:
[[Signals and Systems Lecture 1.pdf#page=8&selection=92,0,199,7|Signals and Systems Lecture 1, page 8]]
$$ F = m \dot{\dot{p}} \ \ \ \begin{cases} x(t) = m\frac{d^2p(t)}{dt^2} \\ y(t) = p(t) \end{cases}$$
Μπορούμε να περιγράψουμε το σύστημα $S$ μέσω μίας διαφορικής εξίσωσης που συσχετίζει τα x, y.  Όπως οι εξισώσεις του Νεύτονα. Αυτά που εκφράζονται με τον τρόπο αυτό ονομάζουμε *δυναμικά*

## Στατικά:
[[Signals and Systems Lecture 1.pdf#page=8&selection=39,4,90,6|Signals and Systems Lecture 1, page 8]]
Αν περιγράφεται με τρόπο όπως τον Νόμο του Ohm: $y(t)=S(x(t))$ τα ονομάζουμε *στατικά*

## Αιτιατά - μη αιτιατά
[[Signals and Systems Lecture 1.pdf#page=9&selection=0,0,59,6|Signals and Systems Lecture 1, page 9]]
Το $y(t)$ εξαρτάται **μόνο** από το $x(e), \ e < t$ 

## Χρονικά αμετάβλητα vs μεταβλητά
[[Signals and Systems Lecture 1.pdf#page=9&selection=61,0,153,6|Signals and Systems Lecture 1, page 9]]
- Αμετάβλητο: $$y(t -t_0) = S(x(t-t_0)), \ \forall t_0 \in R$$
- Μεταβλητό: το ανάποδο...
