1) Si on ne fait pas de ségrégations des interfaces en des composants les plus simples et petits possibles (ISP), on finit pas par ne pas respecter LSP (méthode non implémentée et donc on ne peut pas itérer sur les Printers).

2) Cela forcera à modifier la signature dans SimplePrinter alors qu'il n'implémente même pas cette méthode.

3) Pour palier au probleme on doit creer 4 interfaces Printer,Scanner,Copi,Fax et faire implementer la classe simplePrinter a seulement l'interface Printer .