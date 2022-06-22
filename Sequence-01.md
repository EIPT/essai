---
marp: true
theme: eipt-avance
_class: lead
backgroundColor: #fff
# backgroundImage: url('https://marp.app/assets/hero-background.svg')
# header: 'Header content'
footer: '© 2022: Laurent Marquet/EIPT'
---

# Bachelors Gobelins développeur interactif (BDDI)

## Formation Symfony

![bg vertical left:40% 50%](https://eipt.fr/images/Logos/Logo-EcoleCCI.png)
![bg 70%](https://eipt.fr/images/Logos/Logo-Gobelins.png)
![bg 70%](https://eipt.fr/images/Logos/Logo-EIPT.png)

---

# Séquence 7

## Finalisation du CRUD pour l’Entity et utilisation des Fixtures

## https://run.as/5kn56y

---

## Classes nécessaires et utilité

Quelles sont les classes nécessaires et quelle est leur utilité ?

![w:200 center](https://eipt.fr/images/Personnages/Ali/Ali-08.png)

---

## Essai markdown

```markdown
# Slide 1

foobar

---

# Slide 2

foobar
```

---

```markdown
git status;
git add .; git commit; #Reprendre infos du ChangeLog
git checkout main; git merge dev;
git checkout dev; git tag -a vX.X -m'Version X.X';
git push origin --all; git push origin --tags;
```

---

# titre

```php
//src/Service/CharacterService.php
<?php

namespace App\Service;

use DateTime;
use App\Entity\Character;

class CharacterService implements CharacterServiceInterface
{
    /**
     * {@inheritdoc}
     */
    public function create() {
        $character = new Character();
        $character
            ->setKind('Dame')
            ->setName('Eldalótë')
            ->setSurname('Fleur elfique')
            ->setCaste('Elfe')
            ->setKnowledge('Arts')
            ->setIntelligence(120)
            ->setLife(12)
            ->setImage('/images/eldalote.jpg')
            ->setCreation(new DateTime())
        ;

        return $character;
    }
}
```

---
# I am slide

<style scoped>
pre {
   font-size: 2rem;
}
</style>

```cs
// I am code block
\```

---