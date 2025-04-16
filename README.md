# Quantum Machine Learning - Toxic Comment Classification using VQC 


## Descriere generala
Acest proiect exploreaza aplicarea invatarii automate cuantice (Quantum Machine Learning - QML) pe un task real de clasificare binara, utilizand date din competitia Jigsaw Toxic Comment Classification Challenge (Kaggle). Scopul este clasificarea comentariilor toxice, simplificand problema initiala prin pastrarea unei singure etichete: `toxic`.
**Pentru informatii suplimentare, se pot consulta atat prezentarea atasata in acest repository, cat si notebook-ul in care se afla codul.**
## Obiective
- Compararea performantelor intre un model clasic de tip Logistic Regression si un model cuantic Variational Quantum Classifier (VQC)
- Ilustrarea modului de integrare a circuitelor cuantice in fluxul standard de invatare automata

### Modele utilizate
- Logistic Regression (model clasic de referinta)
- Variational Quantum Classifier (QML, implementat in Qiskit)

## Rezultate

| Model               | Acuratete | Timp procesare |
|---------------------|-----------|----------------|
| Logistic Regression | 93%       | ~6.4 ms        |
| VQC                 | 93%       | ~949 ms        |

Ambele modele au obtinut aceeasi acuratete, insa VQC a fost semnificativ mai lent. Reducerea dimensionalitatii a fost esentiala pentru ca modelul cuantic sa functioneze corespunzator. Acest lucru indica faptul ca, in forma actuala, VQC nu reprezinta o solutie eficienta pentru astfel de sarcini simple, comparativ cu metodele clasice. De altfel, dezvoltarea aplicatiilor de Quantum Machine Learning folosind Qiskit este inca afectata de instabilitatea ecosistemului de librarii. Versiunile acestora nu sunt intotdeauna compatibile intre ele, iar documentatia oficiala nu acopera toate combinatiile posibile. Acest lucru poate ingreuna configurarea mediului de lucru si reproducerea experimentelor, reprezentand o limitare semnificativa, in special in contexte educationale sau de cercetare, unde timpul si resursele sunt limitate.

