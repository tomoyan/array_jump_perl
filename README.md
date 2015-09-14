# array_jump_perl 

Starting at the 0 (zero) index,
you need to "jump" through a one-dimensional array (zero based index)# of true/false values.
True is a place you can land on (if desired)
and false is a place you must jump over (cannot land on).
The array can be very very long.

Your "velocity" indicates how many spots (or array indexes) you advance every jump.
For example, if you have a velocity of 2 and are currently at index 4, after the jump, you will be at index 6.
Before each jump you can increase your velocity by 1, decrease your velocity by 1, or keep the same velocity.
You can only go forwards.

You start at index 0 (zero), with a velocity of 1.
This means that for the very first jump, you can keep the same velocity and move to index 1,
or increase velocity by 1 (to a velocity of 2) to move to index 2.
On this first jump, you can't decrease your velocity as that would make your velocity 0 (zero) and you wouldn't move.
Now that you've jumped, you can again increase, decrease, or keep your velocity the same, then jump again.

As an example, let's say you increased your velocity to 2 and jumped. You're now at index 2 with a velocity of 2. You can:
1.  decrease your velocity to 1 and jump to index 3.
2.  Keep your velocity at 2 and jump to index 4.
3.  Increase your velocity to 3 and jump to index 5.
Remember, you can only jump to an index if it's "true".
You are successful if you can get past the last index.
Implement a function to determine if you can successfully jump through the array.

Here is an array that is NOT passable:
$notPassable = array(true, true, false, true, false, true, false, false, false, true);

Here is an an array that is passable:
$passable = array(true, true, false, true, false, true, true, false, false, true, false);
