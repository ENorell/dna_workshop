# dna_workshop

En introduktion till hur man arbetar med Git och Github. 

## Förberedelser
1. Installera Git: https://git-scm.com/install/
   * Testa installationen genom att köra `git --version` i kommandotolken, PowerShell eller Git Bash
2. Klona detta repository till din dator
   * Från kommandotolken, PowerShell eller Git Bash ställ dig i valfri mapp t.ex. `cd C:/repos`
   * Kör följande kommando för att ladda ned koden `git clone https://github.com/ENorell/dna_workshop.git`
3. Installera Visual Studio Code (VS Code)
   * Installera Git Graph extension (valfritt)
   * Lägg till mappen dna_workshop från steg 2 till ditt workspace i VS Code
   * Du bör kunna se detta repo under "Source Control" i vänstra panelen inuti VS Code
4. Skapa en ny branch med en ändring och puscha (valfritt, vi gör även detta tillsammans)
   * Skapa en egen branch med valfritt namn genom att köra t.ex. `git branch feature/din_branch`
   * Byt till din nya branch genom `git checkout feature/din_branch`
   * Gör en ändring i en existerande fil med valfritt verktyg, t.ex. VS Code
   * Stagea alla dina ändringar med `git add .`
   * Dubbelkolla vilka filer som stageats `git status`
   * Skapa din första commit med ett meddelande t.ex. `git commit -m "emils commit"`
   * Puscha dina ändringar till Github a.k.a remote `git push --set-upstream origin feature/din_branch`

testing
