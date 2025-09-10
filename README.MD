# Présentation

```js
class Developer {
  constructor(username, name, job, programmingLanguages, projects, message) {
    this.username = username;
    this.name = name;
    this.job = job;
    this.programmingLanguages = programmingLanguages;
    this.projects = projects;
    this.message = message;
  }

  details() {
    console.log(`Bonjour, je suis ${this.name} (@${this.username})`);
    console.log(`Statut : ${this.job}`);
    console.log(`Compétences principales : ${this.programmingLanguages.join(', ')}`);
    console.log(this.message);
  }
}

const messageRecruteur = ["## À l'attention des recruteurs", '', 'Mon profil GitHub est utilisé comme un véritable **outil de versionning professionnel**,', 'et non comme un simple espace de stockage ou "FTP".', '', '> Les projets les plus avancés et complexes sont volontairement privés afin de protéger la propriété intellectuelle', '> et éviter toute appropriation commerciale non autorisée.', '', 'Je reste cependant **entièrement disponible pour un entretien technique** durant lequel je pourrai présenter et démontrer mes réalisations privées,', 'afin de témoigner concrètement de mes compétences et de la qualité de mon travail.', '', "Je précise également que le code public est ancien et n'est pas représentatif de la qualité ni de la complexité des projets privés sur lesquels je travaille quotidiennement."].join('\n');

const me = new Developer('RoxasYTB', 'Yohan Sannier', 'Étudiant en informatique | Développeur Full-Stack', ['JavaScript', 'Java', 'Node.js', 'MongoDB', 'HTML/CSS', 'PHP'], [], messageRecruteur);

me.details();
```

---

### Sortie

```txt
Bonjour, je suis Yohan Sannier (@RoxasYTB)
Statut : Étudiant en informatique | Développeur Full-Stack
Compétences principales : JavaScript, Java, Node.js, MongoDB, HTML/CSS, PHP
## À l'attention des recruteurs

Mon profil GitHub est utilisé comme un véritable **outil de versionning professionnel**,
et non comme un simple espace de stockage ou "FTP".

> Les projets les plus avancés et complexes sont volontairement privés afin de protéger la propriété intellectuelle
> et éviter toute appropriation commerciale non autorisée.

Je reste cependant **entièrement disponible pour un entretien technique** durant lequel je pourrai présenter et démontrer mes réalisations privées,
afin de témoigner concrètement de mes compétences et de la qualité de mon travail.

Je précise également que le code public est ancien et n'est pas représentatif de la qualité ni de la complexité des projets privés sur lesquels je travaille quotidiennement.
```

---

## À l'attention des recruteurs

Mon profil GitHub est utilisé comme un véritable **outil de versionning professionnel**, et non comme un simple espace de stockage ou "FTP".

> [!WARNING]  
> Les projets les plus avancés et complexes sont volontairement privés afin de protéger la propriété intellectuelle et éviter toute appropriation commerciale non autorisée.

Je reste cependant **entièrement disponible pour un entretien technique** durant lequel je pourrai présenter et démontrer mes réalisations privées, afin de témoigner concrètement de mes compétences et de la qualité de mon travail.

Je précise également que le **code public** est **ancien** et **n'est pas représentatif de la qualité ni de la complexité des projets privés sur lesquels je travaille quotidiennement.**
