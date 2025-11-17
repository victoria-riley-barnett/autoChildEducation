# Auto Child Education

Automatically assigns optimal education to all children in your country. No configuration needed - just subscribe and play.

## How It Works

**Initial Assignment**: New children are distributed evenly across admin/diplomatic/military (aiming for ~1/3 each type) weighted by any existing trait aptitudes.

**Reassignment**: Every 3 months, children are rechecked. If they gained a trait that doesn't match their education, they switch:
- Admin education + child_gregarious/rowdy/gallant → switches
- Diplomatic education + child_intelligent/rowdy/shrewd → switches  
- Military education + child_intelligent/gregarious/ambitious → switches

**Expensive Education**: Heirs (1000g), crown estate children (2000g), and high-aptitude children (3000g) get expensive education if you can afford it.

**Hardcoded Traits**: Multi-stat traits bypass the normal system:
- child_ambitious → Administrative
- child_gallant → Military
- child_shrewd → Diplomatic

## Why This Approach?

Cabinet value comes from **specialists** (98/82/10) not generalists (80/70/70). Education gives +0.75 to one stat, so matching it to natural trait bonuses (+0.5) creates better cabinet members.

The 3-month recheck catches trait changes (children get traits early in life) while avoiding excessive reassignment.
