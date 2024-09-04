TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados
$ git init
Initialized empty Git repository in F:/Bootcamp-DIO-EngDados/.git/

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados (main)
$ git clone https://github.com/johanngomig/Dio-Bootcamp-EngDados.git
Cloning into 'Dio-Bootcamp-EngDados'...
remote: Enumerating objects: 178, done.
remote: Counting objects: 100% (178/178), done.
remote: Compressing objects: 100% (122/122), done.
remote: Total 178 (delta 37), reused 82 (delta 14), pack-reused 0 (from 0)
Receiving objects: 100% (178/178), 40.54 KiB | 1.50 MiB/s, done.
Resolving deltas: 100% (37/37), done.

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados (main)
$ ls
Dio-Bootcamp-EngDados/

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados (main)
$ cd Dio-Bootcamp-EngDados/

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados (main)
$ ls
README.md  dio-git-e-github/

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados (main)
$ git clone https://github.com/johanngomig/dio-lab-open-source.git
Cloning into 'dio-lab-open-source'...
remote: Enumerating objects: 203704, done.
remote: Counting objects: 100% (78/78), done.
remote: Compressing objects: 100% (49/49), done.
remote: Total 203704 (delta 41), reused 62 (delta 29), pack-reused 203626 (from 1)
Receiving objects: 100% (203704/203704), 169.27 MiB | 17.30 MiB/s, done.
Resolving deltas: 100% (124070/124070), done.
Updating files: 100% (25014/25014), done.

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados (main)
$ ls
README.md  dio-git-e-github/  dio-lab-open-source/

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados (main)
$ cd dio-lab-open-source/

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (main)
$ git remote add upstream https://github.com/digitalinnovationone/dio-lab-open-source.git

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (main)
$ git remote -v
origin  https://github.com/johanngomig/dio-lab-open-source.git (fetch)
origin  https://github.com/johanngomig/dio-lab-open-source.git (push)
upstream        https://github.com/digitalinnovationone/dio-lab-open-source.git (fetch)
upstream        https://github.com/digitalinnovationone/dio-lab-open-source.git (push)

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (main)
$ git pull upstream main
remote: Enumerating objects: 17, done.
remote: Counting objects: 100% (17/17), done.
remote: Compressing objects: 100% (13/13), done.
remote: Total 17 (delta 6), reused 14 (delta 4), pack-reused 0 (from 0)
Unpacking objects: 100% (17/17), 688.53 KiB | 1021.00 KiB/s, done.
From https://github.com/digitalinnovationone/dio-lab-open-source
 * branch                main       -> FETCH_HEAD
 * [new branch]          main       -> upstream/main
Updating 1ce7a425f..7b22a904f
Fast-forward
 community/adolfosorato.md | 35 +++++++++++++++++++++++++++++++++++
 community/jorge-junior.md | 21 +++++++++++++++++++++
 community/t50san.md       | 11 +++++++++++
 3 files changed, 67 insertions(+)
 create mode 100644 community/adolfosorato.md
 create mode 100644 community/jorge-junior.md

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 6 commits.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (main)
$ git checkout -b feat/community/johanngomig
Switched to a new branch 'feat/community/johanngomig'

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (feat/community/johanngomig)
$ touch community/johanngomig.md

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (feat/community/johanngomig)
$ git status
On branch feat/community/johanngomig
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        community/johanngomig.md

nothing added to commit but untracked files present (use "git add" to track)

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (feat/community/johanngomig)
$ git add .

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (feat/community/johanngomig)
$ git status
On branch feat/community/johanngomig
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   community/johanngomig.md


TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (feat/community/johanngomig)
$ git commit -m"Feat: add johanngomig profile"
[feat/community/johanngomig 2d9bd591d] Feat: add johanngomig profile
 1 file changed, 42 insertions(+)
 create mode 100644 community/johanngomig.md

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (feat/community/johanngomig)
$ git log
commit 2d9bd591d47811f6ddb1a4e20f5910965d218dfc (HEAD -> feat/community/johanngomig)
Author: johanngomig <johanngomig@gmail.com>
Date:   Wed Sep 4 14:09:57 2024 -0300

    Feat: add johanngomig profile

commit 7b22a904f9f44477ab7bce6dfaa11b868186e3e6 (upstream/main, main)
Merge: f909d3275 282bae556
Author: github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>
Date:   Wed Sep 4 13:25:44 2024 +0000

    Merge pull request #46794 from jorge-junior/feat/community/jorge-junior

commit 282bae55604ed01373fd390ae9ead964ab00b4b7
Author: Jorge Francisco <91333173+jorge-junior@users.noreply.github.com>
Date:   Wed Sep 4 10:24:28 2024 -0300

    feat: add jorge-junior.md

commit f909d3275e0a4d74596445d7cde87d5d994de314
Merge: 9a2cf3921 d8df356cc
Author: github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>
Date:   Wed Sep 4 13:20:59 2024 +0000

    Merge pull request #46793 from adolfosorato/feat/community/adolfosorato

commit 9a2cf392132aab0eabd10feb3f41e0d673ae7147
Merge: 1ce7a425f ffd90e366
Author: github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>
Date:   Wed Sep 4 13:17:00 2024 +0000

    Merge pull request #46791 from t50san/patch-1

commit ffd90e3665b853bfe1648d45cd815fe188e86a85
Author: Tamires <86693829+t50san@users.noreply.github.com>
Date:   Wed Sep 4 10:15:10 2024 -0300

    Update t50san.md

commit d8df356ccfa9da933432116ec8889a829aefe44d
Author: adolfosorato <adolfosorato@gmail.com>
Date:   Wed Sep 4 10:13:55 2024 -0300

    feat: add adolfosorato profile

commit 1ce7a425f95e528ad7ef6a69fd1beccb76be43d4 (origin/main, origin/HEAD)
Merge: c41de4261 3918e5588
Author: github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>
Date:   Wed Sep 4 12:56:46 2024 +0000

    Merge pull request #46789 from adriana230890/feat/comminuty/adriana230890

commit c41de4261d9f83edc2a802c21c23b5a3c12d2c53
Merge: b400e8599 9ab57233f
Author: github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>
Date:   Wed Sep 4 12:55:40 2024 +0000

    Merge pull request #46788 from kcadu1/feat/community/kcadu1

commit 9ab57233f49e2426d7d4a6b68089e4b5886098cc
Author: kcadu <kcadu2@hotmail.com>
Date:   Wed Sep 4 09:51:07 2024 -0300

    feat: add kcadu1 profile

commit b400e8599835921fa84e8afa6b10fcf44dbbfcb0
Merge: c6090c109 ffd797ba1
Author: github-actions[bot] <41898282+github-actions[bot]@users.noreply.github.com>
Date:   Wed Sep 4 12:37:12 2024 +0000

    Merge pull request #46787 from jeymerson/feat/community/jeymerson

commit ffd797ba11b428383b8799d5c4d271b37c05aea8
Author: Jeymerson <67666280+jeymerson@users.noreply.github.com>
Date:   Wed Sep 4 12:35:28 2024 +0000

    feat: jeymerson profile


TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (feat/community/johanngomig)
$ git push origin feat/community/johanngomig
Enumerating objects: 26, done.
Counting objects: 100% (26/26), done.
Delta compression using up to 16 threads
Compressing objects: 100% (21/21), done.
Writing objects: 100% (21/21), 7.77 KiB | 3.88 MiB/s, done.
Total 21 (delta 11), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (11/11), completed with 3 local objects.
remote:
remote: Create a pull request for 'feat/community/johanngomig' on GitHub by visiting:
remote:      https://github.com/johanngomig/dio-lab-open-source/pull/new/feat/community/johanngomig
remote:
To https://github.com/johanngomig/dio-lab-open-source.git
 * [new branch]          feat/community/johanngomig -> feat/community/johanngomig

TioViking@DESKTOP-9VQ2JFJ MINGW64 /f/Bootcamp-DIO-EngDados/Dio-Bootcamp-EngDados/dio-lab-open-source (feat/community/johanngomig)
$ git branch --list
* feat/community/johanngomig
  main
