# Instructions
Complete the Superhero game by following the steps below (the steps are also listed as TODOs in each class file of the project)
## Steps
1. Add any missing constructors to the Superhero class so that the code in the Main class compiles. Note that the Superhero's life attribute should default to true and the weaponStrength attribute should default to 0.
2. Add any missing methods to the Superhero class so that the code in the Main class compiles.
3. Make sure that each superhero's details are printed out nicely to the command line. Hint: a toString() method can help with this.

Your output be similar to the following to pass the input / output test:

```
public class Superhero {
    private String name;
    private String costume;
    private String weapon;
    private boolean life;
    private int weaponStrength;

    // Constructor with name, costume, and weapon (defaults life to true, weaponStrength to 0)
    public Superhero(String name, String costume, String weapon) {
        this.name = name;
        this.costume = costume;
        this.weapon = weapon;
        this.life = true;
        this.weaponStrength = 0;
    }

    // Overloaded constructor if other parameters (like life and weapon strength) are passed
    public Superhero(String name, String costume, String weapon, boolean life, int weaponStrength) {
        this.name = name;
        this.costume = costume;
        this.weapon = weapon;
        this.life = life;
        this.weaponStrength = weaponStrength;
    }

    // toString() method matching the required output format
    @Override
    public String toString() {
        return "superhero details\n" +
               "name: " + name + "\n" +
               "costume: " + costume + "\n" +
               "weapon: " + weapon + "\n" +
               "life: " + life + "\n" +
               "weapon strength: " + weaponStrength;
    }
}
```
