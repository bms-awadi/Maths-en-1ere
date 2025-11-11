# Formules Générales et Cas Particuliers

## TABLEAU PRINCIPAL

| **Fonction** | **Formule Générale** | **Dérivée Générale** | **Cas Particulier $(U=x)$** | **Dérivée Particulière** | **Remarques** |
|---|---|---|---|---|---|
| **Somme** | $U(x) + V(x)$ | $U'(x) + V'(x)$ | $x + x$ | $1 + 1 = 2$ | Linéarité de la dérivation |
| **Différence** | $U(x) - V(x)$ | $U'(x) - V'(x)$ | $x - x$ | $1 - 1 = 0$ | Cas particulier de la somme |
| **Constante × Fonction** | $k \cdot U(x)$ | $k \cdot U'(x)$ | $k \cdot x$ | $k$ | $k$ indépendant de $x$ |
| **Constante seule** | $k$ | $0$ | $5$ | $0$ | Dérivée toujours nulle |
| **Puissance** | $[U(x)]^n$ | $n \cdot [U(x)]^{n-1} \cdot U'(x)$ | $x^n$ | $n \cdot x^{n-1}$ | Descendre l'exposant |
| **Racine carrée** | $\sqrt{U(x)}$ | $\dfrac{U'(x)}{2\sqrt{U(x)}}$ | $\sqrt{x}$ | $\dfrac{1}{2\sqrt{x}}$ | Equivalent : $U^{1/2}$ |
| **Fraction** | $\dfrac{U(x)}{V(x)}$ | $\dfrac{U'(x) \cdot V(x) - U(x) \cdot V'(x)}{[V(x)]^2}$ | $\dfrac{x}{a}$ | $\dfrac{1}{a}$ | Quotient général |
| **Fraction (Const./Fonction)** | $\dfrac{k}{V(x)}$ | $\dfrac{-k \cdot V'(x)}{[V(x)]^2}$ | $\dfrac{k}{x}$ | $\dfrac{-k}{x^2}$ | Numérateur constant |
| **Fraction (Fonction/Const.)** | $\dfrac{U(x)}{k}$ | $\dfrac{U'(x)}{k}$ | $\dfrac{x}{k}$ | $\dfrac{1}{k}$ | Dénominateur constant |
| **Produit** | $U(x) \cdot V(x)$ | $U'(x) \cdot V(x) + U(x) \cdot V'(x)$ | $x \cdot x$ | $1 \cdot x + x \cdot 1 = 2x$ | Règle du produit |
| **Produit (Const. × Fonction)** | $k \cdot U(x)$ | $k \cdot U'(x)$ | $k \cdot x$ | $k$ | Dérivée linéaire |
| **Composée** | $g(U(x))$ | $g'(U(x)) \cdot U'(x)$ | $g(x)$ | $g'(x)$ | Chaîne de dérivation |

---

## **SYNTHÈSE : QUAND UTILISER QUELLE FORMULE ?**

### **Arbre de décision**

```
Je regarde la structure principale de la fonction

↓

Y a-t-il plusieurs termes séparés par + ou - ?
  ├─ OUI → Dérivée terme par terme (Somme/Différence)
  └─ NON → Continuer

Y a-t-il une puissance (exposant) visible ?
  ├─ OUI → Formule U^n
  └─ NON → Continuer

Y a-t-il une racine (√) ?
  ├─ OUI → Formule √U
  └─ NON → Continuer

Y a-t-il une fraction (numérateur/dénominateur) ?
  ├─ OUI → Formule U/V
  └─ NON → Continuer

Y a-t-il une multiplication de deux fonctions différentes ?
  ├─ OUI → Formule U × V
  └─ NON → C'est peut-être une composée simple

Est-ce une composition (fonction dans fonction) ?
  ├─ OUI → Formule composée g(U)
  └─ NON → Continue...
```

---

## **TABLEAU COMPARATIF : GÉNÉRALE vs PARTICULIÈRE**

### **Pour mieux comprendre la structure**

| Type | Formule Générale | Cas Particulier Simple | Lien |
|---|---|---|---|
| **Puissance** | $f(x) = (2x+1)^5$ → $f'(x) = 5(2x+1)^4 \cdot 2$ | $f(x) = x^5$ → $f'(x) = 5x^4$ | Descendre l'exposant, appliquer chaîne |
| **Racine** | $f(x) = \sqrt{3x-2}$ → $f'(x) = \dfrac{3}{2\sqrt{3x-2}}$ | $f(x) = \sqrt{x}$ → $f'(x) = \dfrac{1}{2\sqrt{x}}$ | Dériver selon $u^{1/2}$ |
| **Fraction** | $f(x) = \dfrac{2x+1}{x^2+1}$ → applique $\dfrac{U'V-UV'}{V^2}$ | $f(x) = \dfrac{5}{x}$ → $f'(x) = \dfrac{-5}{x^2}$ | Cas particulier : $U = k$ |
| **Produit** | $f(x) = (x^2)(x^3) = x^5$ → $f'(x) = 2x \cdot x^3 + x^2 \cdot 3x^2 = 5x^4$ | $f(x) = x \cdot x = x^2$ → $f'(x) = 2x$ | Vérifie la formule |

---

## **AIDE-MÉMOIRE : LES 9 FORMULES ESSENTIELLES**

```
╔════════════════════════════════════════════════════════════════╗
║          LES 9 FORMULES À CONNAÎTRE PAR CŒUR                   ║
╠════════════════════════════════════════════════════════════════╣
║                                                                ║
║  1. SOMME              : (U + V)' = U' + V'                    ║
║                                                                ║
║  2. CONSTANTE × FONCTION : (k·U)' = k·U'                       ║
║                                                                ║
║  3. PUISSANCE          : [U^n]' = n·U^(n-1)·U'                ║
║                                                                ║
║  4. RACINE CARRÉE      : [√U]' = U'/(2√U)                      ║
║                                                                ║
║  5. QUOTIENT           : [U/V]' = (U'V - UV')/V²               ║
║                                                                ║
║  6. PRODUIT            : [U·V]' = U'V + UV'                    ║
║                                                                ║
║  7. COMPOSÉE (CHAÎNE)  : [g(U)]' = g'(U)·U'                    ║
║                                                                ║
║  8. CAS SIMPLE : PUISSANCE    x^n → nx^(n-1)                  ║
║                                                                ║
║  9. CAS SIMPLE : RACINE       √x → 1/(2√x)                    ║
║                                                                ║
╚════════════════════════════════════════════════════════════════╝
```

---

## **CONSEILS PRATIQUES**

### **Avant de dériver, toujours...**

1. ✓ **Identifier la structure** : Somme ? Produit ? Fraction ? Puissance ?
2. ✓ **Repérer les composées** : Qu'est-ce qui est la fonction interne ?
3. ✓ **Écrire la formule** : Avant de calculer, écris la formule appropriée
4. ✓ **Calculer les dérivées intermédiaires** : $U'(x)$, $V'(x)$, etc.
5. ✓ **Substituer dans la formule** : Remplissage méthodique
6. ✓ **Simplifier** : Factoriser, réduire, nettoyer le résultat

### **Erreurs courantes à éviter**

❌ Oublier la chaîne : $(2x)^3 \neq 3 \cdot (2x)^2$ 

✓ C'est : $3(2x)^2 \cdot 2 = 6(2x)^2$

---

❌ Inverser le quotient : $\left(\dfrac{U}{V}\right)' \neq \dfrac{U'}{V'}$

✓ C'est : $\dfrac{U'V - UV'}{V^2}$

---

❌ Oublier un terme dans le produit : $(UV)' \neq U'V$

✓ C'est : $U'V + UV'$ (deux termes !)

---

## **CONCLUSION**

Maîtriser ces 9 formules te permet de dériver **presque n'importe quelle fonction** en 1ère année.

**La clé : Bien identifier la structure, puis appliquer la bonne formule ! 🎯**

