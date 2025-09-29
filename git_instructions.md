The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
Mac:git-essential-training-5988161 dpro$ git add Example.md
Mac:git-essential-training-5988161 dpro$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Example.md

Mac:git-essential-training-5988161 dpro$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Example.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Ex2.md

Mac:git-essential-training-5988161 dpro$ git add Ex
Ex2.md      Example.md  
Mac:git-essential-training-5988161 dpro$ git add Ex
Ex2.md      Example.md  
Mac:git-essential-training-5988161 dpro$ git add Ex2.md 
Mac:git-essential-training-5988161 dpro$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   Ex2.md
        new file:   Example.md

Mac:git-essential-training-5988161 dpro$ git commit -m "adds 2 example markdowns"
[main 381fee5] adds 2 example markdowns
 2 files changed, 2 insertions(+)
 create mode 100644 Ex2.md
 create mode 100644 Example.md
Mac:git-essential-training-5988161 dpro$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
Mac:git-essential-training-5988161 dpro$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 11 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (4/4), 349 bytes | 349.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/kurthuff/git-essential-training-5988161.git
   4bf5834..381fee5  main -> main
Mac:git-essential-training-5988161 dpro$ git pull
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 1.18 KiB | 302.00 KiB/s, done.
From https://github.com/kurthuff/git-essential-training-5988161
   381fee5..dc3f05a  main       -> origin/main
Updating 381fee5..dc3f05a
Fast-forward
 ExPull.md | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 ExPull.md
Mac:git-essential-training-5988161 dpro$ cd projects
bash: cd: projects: No such file or directory
Mac:git-essential-training-5988161 dpro$ cd
Mac:~ dpro$ cd projects
Mac:projects dpro$ cd git-init-example
Mac:git-init-example dpro$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint:
hint:   git config --global init.defaultBranch <name>
hint:
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint:
hint:   git branch -m <name>
hint:
hint: Disable this message with "git config set advice.defaultBranchName false"
Initialized empty Git repository in /Users/dpro/projects/git-init-example/.git/
Mac:git-init-example dpro$ git branch -m main
Mac:git-init-example dpro$ git config --global init.defaultBranch development
Mac:git-init-example dpro$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .DS_Store
        README.md
        literature/
        scripts/

nothing added to commit but untracked files present (use "git add" to track)
Mac:git-init-example dpro$ git add .
Mac:git-init-example dpro$ gitstatus
bash: gitstatus: command not found
Mac:git-init-example dpro$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   .DS_Store
        new file:   README.md
        new file:   literature/Agricultural Biomass Residue Inventories.pdf
        new file:   literature/ian-mcdonald.pdf
        new file:   scripts/.DS_Store
        new file:   scripts/__pycache__/.DS_Store
        new file:   scripts/__pycache__/masc_scrape.cpython-313.pyc
        new file:   scripts/attach_pixels_to_masc.py
        new file:   scripts/biomass_rasters_build.py
        new file:   scripts/filter_towns_over5000.py
        new file:   scripts/make_agol_gpkg.py
        new file:   scripts/masc_agg_redist_pixel_nans.py
        new file:   scripts/masc_agg_scrape.py
        new file:   scripts/masc_prepare.py
        new file:   scripts/masc_scrape.py
        new file:   scripts/merge_radii_to_centroids.py
        new file:   scripts/rasterize_muni_to_aci_grid.py
        new file:   scripts/section_centroids_20km_spacing.py
        new file:   scripts/summarize_centroids_radii_100km.py
        new file:   scripts/summarize_centroids_radii_200km.py
        new file:   scripts/summarize_centroids_radii_20km.py
        new file:   scripts/summarize_centroids_radii_50km.py

Mac:git-init-example dpro$ git commit
Aborting commit due to empty commit message.
Mac:git-init-example dpro$ git commit -m "initial commit"
[main (root-commit) 4a7bba5] initial commit
 22 files changed, 3595 insertions(+)
 create mode 100644 .DS_Store
 create mode 100644 README.md
 create mode 100644 literature/Agricultural Biomass Residue Inventories.pdf
 create mode 100644 literature/ian-mcdonald.pdf
 create mode 100644 scripts/.DS_Store
 create mode 100644 scripts/__pycache__/.DS_Store
 create mode 100644 scripts/__pycache__/masc_scrape.cpython-313.pyc
 create mode 100644 scripts/attach_pixels_to_masc.py
 create mode 100644 scripts/biomass_rasters_build.py
 create mode 100644 scripts/filter_towns_over5000.py
 create mode 100644 scripts/make_agol_gpkg.py
 create mode 100644 scripts/masc_agg_redist_pixel_nans.py
 create mode 100644 scripts/masc_agg_scrape.py
 create mode 100644 scripts/masc_prepare.py
 create mode 100644 scripts/masc_scrape.py
 create mode 100644 scripts/merge_radii_to_centroids.py
 create mode 100644 scripts/rasterize_muni_to_aci_grid.py
 create mode 100644 scripts/section_centroids_20km_spacing.py
 create mode 100644 scripts/summarize_centroids_radii_100km.py
 create mode 100644 scripts/summarize_centroids_radii_200km.py
 create mode 100644 scripts/summarize_centroids_radii_20km.py
 create mode 100644 scripts/summarize_centroids_radii_50km.py
Mac:git-init-example dpro$ git remote add origin https://github.com/kurthuff/git-init-example.git
Mac:git-init-example dpro$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Mac:git-init-example dpro$ git push --set-upstream origin main
Enumerating objects: 27, done.
Counting objects: 100% (27/27), done.
Delta compression using up to 11 threads
Compressing objects: 100% (27/27), done.
Writing objects: 100% (27/27), 4.82 MiB | 8.21 MiB/s, done.
Total 27 (delta 6), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (6/6), done.
To https://github.com/kurthuff/git-init-example.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
Mac:git-init-example dpro$ 