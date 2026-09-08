## Question 2 : Qu'est-ce qu'une classe abstraite ?

Une classe abstraite est une classe qui ne peut pas être instanciée (on ne peut pas créer d'objet directement avec new). Elle sert de modèle pour d'autres classes. Elle peut contenir à la fois des méthodes concrètes (avec une implémentation) et des méthodes abstraites (déclarées avec le mot-clé abstract, sans corps, qui devront être implémentées par les sous-classes concrètes).

Exemple :
java

// Classe abstraite
public abstract class Vehicule {
    private String marque;

    public Vehicule(String marque) {
        this.marque = marque;
    }

    // Méthode concrète
    public void demarrer() {
        System.out.println("Le véhicule " + marque + " démarre.");
    }

    // Méthode abstraite (sans implémentation)
    public abstract void getNbRoues()[reference:7];
}

