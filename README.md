# GIT-Workshop

En introduktion till hur man arbetar med Git och Github. 

## Förberedelser
1. Skapa ett konto på Github
   * Behövs för att ni ska få puscha till Github (ni kan dock jobba lokalt utan)
   * Vi ger åtkomst till dessa konton när vi ses
2. Installera Git: https://git-scm.com/install/
   * Klicka dig hela vägen igenom installationen
   * Testa installationen genom att köra `git --version` i kommandotolken, PowerShell eller Git Bash
3. Klona detta repository till din dator
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
4. Sätt ditt användarnamn och mail om du inte gjort det tidigare
   * `git config --global user.name "Mona Lisa"`
   * `git config --global user.email "mona.lisa@gmail.com"`
5. Installera Visual Studio Code (VS Code)
   * Lägg till mappen dna_workshop från steg 2 till ditt workspace (File > Add Folder to Workspace)
   * Du bör kunna se detta repo under "Source Control" i vänstra panelen (kan dröja ett par minuter)
   * Installera Git Graph extension
   * Testa extensionen genom att trycka på den nya knappen dyker upp i Source Control brevid namnet på repot

## Övningar på workshoppen
**A) Utveckla och merga din kod in i main-branchen**
   1. Skapa en egen branch med valfritt namn genom att köra t.ex. `git branch feature/din_branch`
   2. Byt till din nya branch genom `git checkout feature/din_branch`
   3. Gör en ändring i en existerande fil med valfritt verktyg, t.ex. VS Code eller Notepad
   4. Stagea alla dina ändringar med `git add .`
   5. Dubbelkolla vilka filer som stageats `git status`
   6. Skapa din första commit med ett meddelande t.ex. `git commit -m "emils commit"`
   7. Puscha dina ändringar till Github a.k.a remote `git push --set-upstream origin feature/din_branch` (räcker vanligtvis med `git push` ifall branchen redan finns i Github)
   8. Skapa en Pull Request med din branch -> `main`
   9. Här sker vanligtvis en "code review" från 2 andra kollegor som behöver godkänna din kod
   10. Merga din kod, men välj "squash merge"

**B) Hämta ändringar i main sen du skapade din branch och hantera merge-konflikter**
   * Upprepa steg 1-6 från övning A
   * Ändra en fil på samma ställe som gjorts i en commit som kommit in till main sen du gjorde din branch
   * Hämta ändringar från main till din branch med `git pull origin main`
   * Ifall ändringar har gjorts kring samma kod så kan en "merge conflict" uppstå, VS Code har ett verktyg för att lösa konflikterna

