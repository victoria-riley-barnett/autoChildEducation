# Auto Child Education

Automatically assigns optimal education to all children in your country.

## How It Works

**Initial Assignment**: New children are distributed evenly across admin/diplomatic/military (aiming for ~1/3 each type) weighted by any existing trait aptitudes. This captures your idiots and prodigies -- all of the general cases are just used to rebalance the distribution.

**Reassignment**: Every 3 months, children are rechecked. If they gained a trait that doesn't match their education, they switch:
- Admin education + child_gregarious → Diplomatic
- Admin education + child_rowdy → Military
- Admin education + child_gallant → Military
- Diplomatic education + child_intelligent → Administrative
- Diplomatic education + child_rowdy → Military
- Military education + child_intelligent → Administrative
- Military education + child_gregarious → Diplomatic
- Military education + child_ambitious → Administrative

**Expensive Education**: Heirs (1000g check), crown estate children (2000g check), and high-aptitude children (3000g check) get expensive education if you can afford it.

**Hardcoded Traits**: Multi-stat traits bypass the normal system in a flavorful way:
- child_ambitious → Administrative, future ruler focus
- child_gallant → Military, chivalric focus
- child_shrewd → Diplomatic, cunning strategist focus