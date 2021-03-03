---
title: Home
order: 0
type: overview
---

<ContentColumn>

# ArcaneExploration

Some cool stuff that we will write here.

--------------------------------

## API

(Hey, we can use code blocks too!)
```java
public class ExampleMob extends Mob {
    
    public TestZombie() {
        // Set the ID to "EXAMPLE_MOB", have a red name of "Example". The Mob is a Zombie and it has 60 health.
        super("EXAMPLE_MOB", ChatColor.RED + "Example", EntityType.ZOMBIE, 60);
    }

    @Override
    public void onSpawn(@Nonnull LivingEntity self, @Nonnull BlockPosition position) {
        // Set the zombie to glow
        self.setGlowing(true);
        // Set that the zombie cannot pick up items
        self.setCanPickupItems(false);
        // Change the movement speed to 2
        self.getAttribute(Attribute.GENERIC_MOVEMENT_SPEED).setBaseValue(2);
    }
}
```
</ContentColumn>
