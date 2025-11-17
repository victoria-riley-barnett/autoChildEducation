# Auto Child Education

Automatically assigns optimal education to all children in your country based on their trait modifiers.

## How It Works

Every month, all children are evaluated by calculating their base aptitude modifiers (subtracting current education bonuses) and assigned to the education type matching their highest base modifier.

The system calculates base modifiers by removing education bonuses then comparing base values (trait values).

Examples:
- Intelligent child (base adm +0.5) → Administrative education
- Rowdy child (base mil +0.5) → Military education  
- Ambitious child (base adm +0.33, dip +0.3) → Administrative education (0.33 > 0.30)
- Gallant child (base dip +0.33, mil +0.33) → Diplomatic education (tie-breaker)
- Shrewd child (base mil +0.33, adm +0.33) → Military education (tie-breaker)
- Prodigy child (base all +1.5) → Cycles through all three types for even distribution

**Expensive Education**: 

Heirs (1000g threshold), crown estate children (2000g threshold), and high-aptitude children (3000g threshold) get expensive education if you can afford it. Children with negative total modifiers (slow/idiot) are excluded.

## Philosophy

Creates specialists (98/75/20) rather than generalists (80/80/80). With 3-6 cabinet slots, you want the best admin advisor, best diplomat, and best general - not six mediocre courtiers.

## Links

Fully open-source, contributions welcome:
- GitHub: https://github.com/victoria-riley-barnett/autoChildEducation
- Steam: https://steamcommunity.com/sharedfiles/filedetails/?id=3607293096

Please report any bugs or edge cases!
