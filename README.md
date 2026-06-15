# Pipeline_Practice


The default interactive shell is now zsh.
To update your account to use zsh, please run `chsh -s /bin/zsh`.
For more details, please visit https://support.apple.com/kb/HT208050.
(base) rajnishatrismbp:pipeline rajnishkhatri$ git init 
Initialized empty Git repository in /Users/rajnishkhatri/Desktop/pipeline/.git/
(base) rajnishatrismbp:pipeline rajnishkhatri$ git add .
(base) rajnishatrismbp:pipeline rajnishkhatri$ git commit -m "new commit for pipeline"
[main (root-commit) 0ff5fd6] new commit for pipeline
 1 file changed, 1 insertion(+)
 create mode 100644 abc.txt
(base) rajnishatrismbp:pipeline rajnishkhatri$ git remote add origin https://github.com/NeetuSDET/Pipeline_Practice.git
(base) rajnishatrismbp:pipeline rajnishkhatri$ git push origin main
To https://github.com/NeetuSDET/Pipeline_Practice.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/NeetuSDET/Pipeline_Practice.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
(base) rajnishatrismbp:pipeline rajnishkhatri$ git pull origin main --rebase
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 872 bytes | 174.00 KiB/s, done.
From https://github.com/NeetuSDET/Pipeline_Practice
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
Successfully rebased and updated refs/heads/main.
(base) rajnishatrismbp:pipeline rajnishkhatri$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 300 bytes | 300.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/NeetuSDET/Pipeline_Practice.git
   a8de46c..405e6ce  main -> main
(base) rajnishatrismbp:pipeline rajnishkhatri$ git branch
* main
(base) rajnishatrismbp:pipeline rajnishkhatri$ npm playwright init@latest
Unknown command: "playwright"

To see a list of supported npm commands, run:
  npm help
(base) rajnishatrismbp:pipeline rajnishkhatri$ npm init playwright@latest

> npx
> "create-playwright"

Getting started with writing end-to-end tests with Playwright:
Initializing project in '.'
✔ Do you want to use TypeScript or JavaScript? · JavaScript
✔ Where to put your end-to-end tests? · tests
✔ Add a GitHub Actions workflow? (Y/n) · true
✔ Install Playwright browsers (can be done manually via 'npx playwright install')? (Y/n) · true

Initializing NPM project (npm init -y)…
Wrote to /Users/rajnishkhatri/Desktop/pipeline/package.json:

{
  "name": "pipeline",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/NeetuSDET/Pipeline_Practice.git"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "type": "commonjs",
  "bugs": {
    "url": "https://github.com/NeetuSDET/Pipeline_Practice/issues"
  },
  "homepage": "https://github.com/NeetuSDET/Pipeline_Practice#readme"
}


Installing Playwright Test (npm install --save-dev @playwright/test)…

added 3 packages, and audited 4 packages in 17s

found 0 vulnerabilities
Installing Types (npm install --save-dev @types/node)…

added 3 packages, and audited 7 packages in 2s

found 0 vulnerabilities
Writing playwright.config.js.
Writing .github/workflows/playwright.yml.
Writing tests/example.spec.js.
Writing package.json.
Downloading browsers (npx playwright install)…
Downloading Chrome for Testing 149.0.7827.55 (playwright chromium v1228) from https://cdn.playwright.dev/builds/cft/149.0.7827.55/mac-arm64/chrome-mac-arm64.zip
171 MiB [====================] 100% 0.0s
Chrome for Testing 149.0.7827.55 (playwright chromium v1228) downloaded to /Users/rajnishkhatri/Library/Caches/ms-playwright/chromium-1228
Downloading Chrome Headless Shell 149.0.7827.55 (playwright chromium-headless-shell v1228) from https://cdn.playwright.dev/builds/cft/149.0.7827.55/mac-arm64/chrome-headless-shell-mac-arm64.zip
93.5 MiB [====================] 100% 0.0s
Chrome Headless Shell 149.0.7827.55 (playwright chromium-headless-shell v1228) downloaded to /Users/rajnishkhatri/Library/Caches/ms-playwright/chromium_headless_shell-1228
Downloading Firefox 151.0 (playwright firefox v1532) from https://cdn.playwright.dev/dbazure/download/playwright/builds/firefox/1532/firefox-mac-arm64.zip
98.8 MiB [====================] 100% 0.0s
Firefox 151.0 (playwright firefox v1532) downloaded to /Users/rajnishkhatri/Library/Caches/ms-playwright/firefox-1532
Downloading WebKit 26.5 (playwright webkit v2311) from https://cdn.playwright.dev/dbazure/download/playwright/builds/webkit/2311/webkit-mac-15-arm64.zip
77.2 MiB [====================] 100% 0.0s
WebKit 26.5 (playwright webkit v2311) downloaded to /Users/rajnishkhatri/Library/Caches/ms-playwright/webkit-2311
✔ Success! Created a Playwright Test project at /Users/rajnishkhatri/Desktop/pipeline

Inside that directory, you can run several commands:

  npx playwright test
    Runs the end-to-end tests.

  npx playwright test --ui
    Starts the interactive UI mode.

  npx playwright test --project=chromium
    Runs the tests only on Desktop Chrome.

  npx playwright test example
    Runs the tests in a specific file.

  npx playwright test --debug
    Runs the tests in debug mode.

  npx playwright codegen
    Auto generate tests with Codegen.

We suggest that you begin by typing:

    npx playwright test

And check out the following files:
  - ./tests/example.spec.js - Example end-to-end test
  - ./playwright.config.js - Playwright Test configuration

Visit https://playwright.dev/docs/intro for more information. ✨

Happy hacking! 🎭
(base) rajnishatrismbp:pipeline rajnishkhatri$ npx playwright test

Running 6 tests using 4 workers
  6 passed (22.9s)

To open last HTML report run:

  npx playwright show-report

(base) rajnishatrismbp:pipeline rajnishkhatri$ npx plawright test tests/task.spec.js
npm error code E404
npm error 404 Not Found - GET https://registry.npmjs.org/plawright - Not found
npm error 404
npm error 404  The requested resource 'plawright@*' could not be found or you do not have permission to access it.
npm error 404
npm error 404 Note that you can also install from a
npm error 404 tarball, folder, http url, or git url.
npm error A complete log of this run can be found in: /Users/rajnishkhatri/.npm/_logs/2026-06-15T14_59_50_277Z-debug-0.log
(base) rajnishatrismbp:pipeline rajnishkhatri$ npx plawright test tests/task.spec.js --headed
npm error code E404
npm error 404 Not Found - GET https://registry.npmjs.org/plawright - Not found
npm error 404
npm error 404  The requested resource 'plawright@*' could not be found or you do not have permission to access it.
npm error 404
npm error 404 Note that you can also install from a
npm error 404 tarball, folder, http url, or git url.
npm error A complete log of this run can be found in: /Users/rajnishkhatri/.npm/_logs/2026-06-15T15_00_10_892Z-debug-0.log
(base) rajnishatrismbp:pipeline rajnishkhatri$ npx plawright test tests/task.spec.js --headed
npm error code E404
npm error 404 Not Found - GET https://registry.npmjs.org/plawright - Not found
npm error 404
npm error 404  The requested resource 'plawright@*' could not be found or you do not have permission to access it.
npm error 404
npm error 404 Note that you can also install from a
npm error 404 tarball, folder, http url, or git url.
npm error A complete log of this run can be found in: /Users/rajnishkhatri/.npm/_logs/2026-06-15T15_00_26_479Z-debug-0.log
(base) rajnishatrismbp:pipeline rajnishkhatri$ npx playwright test npx playwright test tests/task.spec.js --headed

Running 9 tests using 4 workers
  1) [chromium] › tests/task.spec.js:3:5 › Search Product ──────────────────────────────────────────

    Error: locator.fill: Error: strict mode violation: getByPlaceholder('Search for Products, Brands and More') resolved to 2 elements:
        1) <input name="q" value="" type="text" autocomplete="off" class="nw1UBF v1zwn25" title="Search for Products, Brands and More" placeholder="Search for Products, Brands and More"/> aka getByRole('textbox', { name: 'Search for Products, Brands' })
        2) <input readonly name="q" value="" type="text" autocomplete="off" class="nw1UBF v1zwn25" title="Search for Products, Brands and More" placeholder="Search for Products, Brands and More"/> aka locator('a').filter({ hasText: 'Search Icon' }).getByPlaceholder('Search for Products, Brands')

    Call log:
      - waiting for getByPlaceholder('Search for Products, Brands and More')


      4 |
      5 |     await page.goto('https://www.flipkart.com/')
    > 6 |     await page.getByPlaceholder('Search for Products, Brands and More').fill('iphone 15')
        |                                                                         ^
      7 |     await page.locator('button[type="submit"]').click()
      8 |
      9 |
        at /Users/rajnishkhatri/Desktop/pipeline/tests/task.spec.js:6:73

    Error Context: test-results/task-Search-Product-chromium/error-context.md

  2) [webkit] › tests/task.spec.js:3:5 › Search Product ────────────────────────────────────────────

    Error: locator.fill: Error: strict mode violation: getByPlaceholder('Search for Products, Brands and More') resolved to 2 elements:
        1) <input name="q" value="" type="text" autocomplete="off" class="nw1UBF v1zwn25" title="Search for Products, Brands and More" placeholder="Search for Products, Brands and More"/> aka getByRole('textbox', { name: 'Search for Products, Brands' })
        2) <input readonly name="q" value="" type="text" autocomplete="off" class="nw1UBF v1zwn25" title="Search for Products, Brands and More" placeholder="Search for Products, Brands and More"/> aka locator('a').filter({ hasText: 'Search Icon' }).getByPlaceholder('Search for Products, Brands')

    Call log:
      - waiting for getByPlaceholder('Search for Products, Brands and More')


      4 |
      5 |     await page.goto('https://www.flipkart.com/')
    > 6 |     await page.getByPlaceholder('Search for Products, Brands and More').fill('iphone 15')
        |                                                                         ^
      7 |     await page.locator('button[type="submit"]').click()
      8 |
      9 |
        at /Users/rajnishkhatri/Desktop/pipeline/tests/task.spec.js:6:73

    Error Context: test-results/task-Search-Product-webkit/error-context.md

  3) [firefox] › tests/task.spec.js:3:5 › Search Product ───────────────────────────────────────────

    Error: locator.fill: Error: strict mode violation: getByPlaceholder('Search for Products, Brands and More') resolved to 2 elements:
        1) <input name="q" value="" type="text" autocomplete="off" class="nw1UBF v1zwn25" title="Search for Products, Brands and More" placeholder="Search for Products, Brands and More"/> aka getByRole('textbox', { name: 'Search for Products, Brands' })
        2) <input readonly name="q" value="" type="text" autocomplete="off" class="nw1UBF v1zwn25" title="Search for Products, Brands and More" placeholder="Search for Products, Brands and More"/> aka locator('a').filter({ hasText: 'Search Icon' }).getByPlaceholder('Search for Products, Brands')

    Call log:
      - waiting for getByPlaceholder('Search for Products, Brands and More')


      4 |
      5 |     await page.goto('https://www.flipkart.com/')
    > 6 |     await page.getByPlaceholder('Search for Products, Brands and More').fill('iphone 15')
        |                                                                         ^
      7 |     await page.locator('button[type="submit"]').click()
      8 |
      9 |
        at /Users/rajnishkhatri/Desktop/pipeline/tests/task.spec.js:6:73

    Error Context: test-results/task-Search-Product-firefox/error-context.md

  3 failed
    [chromium] › tests/task.spec.js:3:5 › Search Product ───────────────────────────────────────────
    [firefox] › tests/task.spec.js:3:5 › Search Product ────────────────────────────────────────────
    [webkit] › tests/task.spec.js:3:5 › Search Product ─────────────────────────────────────────────
  6 passed (28.4s)

  Serving HTML report at http://localhost:9323. Press Ctrl+C to quit.
^C
(base) rajnishatrismbp:pipeline rajnishkhatri$ npx playwright test npx playwright test tests/task.spec.js --headed

Running 9 tests using 4 workers
  1) [chromium] › tests/task.spec.js:3:5 › Search Product ──────────────────────────────────────────

    Test timeout of 30000ms exceeded.

    Error: locator.click: Test timeout of 30000ms exceeded.
    Call log:
      - waiting for locator('button[type="submit"]')
        - locator resolved to <button type="submit" class="XFwMiH" title="Search for Products, Brands and More" aria-label="Search for Products, Brands and More">…</button>
      - attempting click action
        2 × waiting for element to be visible, enabled and stable
          - element is visible, enabled and stable
          - scrolling into view if needed
          - done scrolling
          - <div tabindex="-1" class="mcO4kT RFBkxv">…</div> intercepts pointer events
        - retrying click action
        - waiting 20ms
        2 × waiting for element to be visible, enabled and stable
          - element is visible, enabled and stable
          - scrolling into view if needed
          - done scrolling
          - <div tabindex="-1" class="mcO4kT RFBkxv">…</div> intercepts pointer events
        - retrying click action
          - waiting 100ms
        49 × waiting for element to be visible, enabled and stable
           - element is visible, enabled and stable
           - scrolling into view if needed
           - done scrolling
           - <div tabindex="-1" class="mcO4kT RFBkxv">…</div> intercepts pointer events
         - retrying click action
           - waiting 500ms


       6 |     await page.getByRole('textbox', { name: 'Search for Products, Brands' }).fill('iphone');
       7 |
    >  8 |     await page.locator('button[type="submit"]').click()
         |                                                 ^
       9 |
      10 |
      11 | })
        at /Users/rajnishkhatri/Desktop/pipeline/tests/task.spec.js:8:49

    Error Context: test-results/task-Search-Product-chromium/error-context.md

  2) [firefox] › tests/task.spec.js:3:5 › Search Product ───────────────────────────────────────────

    Test timeout of 30000ms exceeded.

    Error: locator.click: Test timeout of 30000ms exceeded.
    Call log:
      - waiting for locator('button[type="submit"]')
        - locator resolved to <button type="submit" class="XFwMiH" title="Search for Products, Brands and More" aria-label="Search for Products, Brands and More">…</button>
      - attempting click action
        2 × waiting for element to be visible, enabled and stable
          - element is visible, enabled and stable
          - scrolling into view if needed
          - done scrolling
          - <div tabindex="-1" class="mcO4kT RFBkxv">…</div> intercepts pointer events
        - retrying click action
        - waiting 20ms
        2 × waiting for element to be visible, enabled and stable
          - element is visible, enabled and stable
          - scrolling into view if needed
          - done scrolling
          - <div tabindex="-1" class="mcO4kT RFBkxv">…</div> intercepts pointer events
        - retrying click action
          - waiting 100ms
        45 × waiting for element to be visible, enabled and stable
           - element is visible, enabled and stable
           - scrolling into view if needed
           - done scrolling
           - <div tabindex="-1" class="mcO4kT RFBkxv">…</div> intercepts pointer events
         - retrying click action
           - waiting 500ms


       6 |     await page.getByRole('textbox', { name: 'Search for Products, Brands' }).fill('iphone');
       7 |
    >  8 |     await page.locator('button[type="submit"]').click()
         |                                                 ^
       9 |
      10 |
      11 | })
        at /Users/rajnishkhatri/Desktop/pipeline/tests/task.spec.js:8:49

    Error Context: test-results/task-Search-Product-firefox/error-context.md

  3) [webkit] › tests/task.spec.js:3:5 › Search Product ────────────────────────────────────────────

    Test timeout of 30000ms exceeded.

    Error: locator.click: Test timeout of 30000ms exceeded.
    Call log:
      - waiting for locator('button[type="submit"]')
        - locator resolved to <button type="submit" class="XFwMiH" title="Search for Products, Brands and More" aria-label="Search for Products, Brands and More">…</button>
      - attempting click action
        2 × waiting for element to be visible, enabled and stable
          - element is visible, enabled and stable
          - scrolling into view if needed
          - done scrolling
          - <div tabindex="-1" class="mcO4kT RFBkxv">…</div> intercepts pointer events
        - retrying click action
        - waiting 20ms
        2 × waiting for element to be visible, enabled and stable
          - element is visible, enabled and stable
          - scrolling into view if needed
          - done scrolling
          - <div tabindex="-1" class="mcO4kT RFBkxv">…</div> intercepts pointer events
        - retrying click action
          - waiting 100ms
        47 × waiting for element to be visible, enabled and stable
           - element is visible, enabled and stable
           - scrolling into view if needed
           - done scrolling
           - <div tabindex="-1" class="mcO4kT RFBkxv">…</div> intercepts pointer events
         - retrying click action
           - waiting 500ms


       6 |     await page.getByRole('textbox', { name: 'Search for Products, Brands' }).fill('iphone');
       7 |
    >  8 |     await page.locator('button[type="submit"]').click()
         |                                                 ^
       9 |
      10 |
      11 | })
        at /Users/rajnishkhatri/Desktop/pipeline/tests/task.spec.js:8:49

    Error Context: test-results/task-Search-Product-webkit/error-context.md

  3 failed
    [chromium] › tests/task.spec.js:3:5 › Search Product ───────────────────────────────────────────
    [firefox] › tests/task.spec.js:3:5 › Search Product ────────────────────────────────────────────
    [webkit] › tests/task.spec.js:3:5 › Search Product ─────────────────────────────────────────────
  6 passed (44.0s)

  Serving HTML report at http://localhost:9323. Press Ctrl+C to quit.
^C
(base) rajnishatrismbp:pipeline rajnishkhatri$ npx playwright test npx playwright test tests/task.spec.js --headed

Running 9 tests using 4 workers
  9 passed (19.4s)

To open last HTML report run:

  npx playwright show-report

(base) rajnishatrismbp:pipeline rajnishkhatri$ git add .
(base) rajnishatrismbp:pipeline rajnishkhatri$ git commit -m "new commit for pipeline"
[main 96ff2b3] new commit for pipeline
 7 files changed, 265 insertions(+)
 create mode 100644 .github/workflows/playwright.yml
 create mode 100644 .gitignore
 create mode 100644 package-lock.json
 create mode 100644 package.json
 create mode 100644 playwright.config.js
 create mode 100644 tests/example.spec.js
 create mode 100644 tests/task.spec.js
(base) rajnishatrismbp:pipeline rajnishkhatri$ git remote add origin https://github.com/NeetuSDET/Pipeline_Practice.git
error: remote origin already exists.
(base) rajnishatrismbp:pipeline rajnishkhatri$ git push origin main
Enumerating objects: 13, done.
Counting objects: 100% (13/13), done.
Delta compression using up to 8 threads
Compressing objects: 100% (10/10), done.
Writing objects: 100% (12/12), 3.56 KiB | 3.56 MiB/s, done.
Total 12 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/NeetuSDET/Pipeline_Practice.git
   405e6ce..96ff2b3  main -> main
(base) rajnishatrismbp:pipeline rajnishkhatri$ git add .
(base) rajnishatrismbp:pipeline rajnishkhatri$ git add Jenkinsfile
(base) rajnishatrismbp:pipeline rajnishkhatri$ git commit -m "commit for pipelin repo"
[main d836541] commit for pipelin repo
 2 files changed, 88 insertions(+)
 create mode 100644 Jenkinfile
 create mode 100644 Jenkinsfile
(base) rajnishatrismbp:pipeline rajnishkhatri$ git push origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 586 bytes | 586.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/NeetuSDET/Pipeline_Practice.git
   96ff2b3..d836541  main -> main
(base) rajnishatrismbp:pipeline rajnishkhatri$ node -v
v23.10.0
(base) rajnishatrismbp:pipeline rajnishkhatri$ pipeline {
    agent any

    environment {
        PATH = "/opt/homebrew/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    }

    stages {
        stage('Checkout') {
            steps {
        bash: pipeline: command not found
        git branch: 'main', url: 'https://github.c(base) rajnishatrismbp:pipeline rajnishkhatri$     agent any

    environment {
        PATH = "/opt/homebrew/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NeetuSDET/Pipeline_Practice.git'
            }
        }

        stage('Install Dependencies') {bash: agent: command not found
(base) rajnishatrismbp:pipeline rajnishkhatri$ 
    environment {
        PATH = "/opt/homebrew/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NeetuSDET/Pipeline_Practice.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm insta(base) rajnishatrismbp:pipeline rajnishkhatri$     environment {
        PATH = "/opt/homebrew/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NeetuSDET/Pipeline_Practice.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Instalbash: environment: command not found
(base) rajnishatrismbp:pipeline rajnishkhatri$         PATH = "/opt/homebrew/bin:/usr/local/bin:/usr/bin:/bin:/usr/sbin:/sbin"
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NeetuSDET/Pipeline_Practice.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Install Playwright Browsers') {
            steps {
                sh 'npx playwright install'
          bash: PATH: command not found
  }
        }

        stage('Run Tests') {
      (base) rajnishatrismbp:pipeline rajnishkhatri$     }
bash: syntax error near unexpected token `}'

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NeetuSDET/Pipeline_Practice.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Install Playwright Browsers') {
            steps {
                sh 'npx playwright install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npx playwright t(base) rajnishatrismbp:pipeline rajnishkhatri$ 
(base) rajnishatrismbp:pipeline rajnishkhatri$     stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/NeetuSDET/Pipeline_Practice.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Install Playwright Browsers') {
            steps {
                sh 'npx playwright install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npx playwright test'
            }
        }
    }
}bash: stages: command not found
(base) rajnishatrismbp:pipeline rajnishkhatri$         stage('Checkout') {
bash: syntax error near unexpected token `'Checkout''
(base) rajnishatrismbp:pipeline rajnishkhatri$             steps {
bash: steps: command not found
(base) rajnishatrismbp:pipeline rajnishkhatri$                 git branch: 'main', url: 'https://github.com/NeetuSDET/Pipeline_Practice.git'
git: 'branch:' is not a git command. See 'git --help'.

The most similar command is
        branch
(base) rajnishatrismbp:pipeline rajnishkhatri$             }
bash: syntax error near unexpected token `}'
(base) rajnishatrismbp:pipeline rajnishkhatri$         }
bash: syntax error near unexpected token `}'
(base) rajnishatrismbp:pipeline rajnishkhatri$ 
(base) rajnishatrismbp:pipeline rajnishkhatri$         stage('Install Dependencies') {
bash: syntax error near unexpected token `'Install Dependencies''
(base) rajnishatrismbp:pipeline rajnishkhatri$             steps {
bash: steps: command not found
(base) rajnishatrismbp:pipeline rajnishkhatri$                 sh 'npm install'
sh: npm install: No such file or directory
(base) rajnishatrismbp:pipeline rajnishkhatri$             }
bash: syntax error near unexpected token `}'
(base) rajnishatrismbp:pipeline rajnishkhatri$         }
bash: syntax error near unexpected token `}'
(base) rajnishatrismbp:pipeline rajnishkhatri$ 
(base) rajnishatrismbp:pipeline rajnishkhatri$         stage('Install Playwright Browsers') {
bash: syntax error near unexpected token `'Install Playwright Browsers''
(base) rajnishatrismbp:pipeline rajnishkhatri$             steps {
bash: steps: command not found
(base) rajnishatrismbp:pipeline rajnishkhatri$                 sh 'npx playwright install'
sh: npx playwright install: No such file or directory
(base) rajnishatrismbp:pipeline rajnishkhatri$             }
bash: syntax error near unexpected token `}'
(base) rajnishatrismbp:pipeline rajnishkhatri$         }
bash: syntax error near unexpected token `}'
(base) rajnishatrismbp:pipeline rajnishkhatri$ 
(base) rajnishatrismbp:pipeline rajnishkhatri$         stage('Run Tests') {
bash: syntax error near unexpected token `'Run Tests''
(base) rajnishatrismbp:pipeline rajnishkhatri$             steps {
bash: steps: command not found
(base) rajnishatrismbp:pipeline rajnishkhatri$                 sh 'npx playwright test'
sh: npx playwright test: No such file or directory
(base) rajnishatrismbp:pipeline rajnishkhatri$             }
bash: syntax error near unexpected token `}'
(base) rajnishatrismbp:pipeline rajnishkhatri$         }
bash: syntax error near unexpected token `}'
(base) rajnishatrismbp:pipeline rajnishkhatri$     }
bash: syntax error near unexpected token `}'
(base) rajnishatrismbp:pipeline rajnishkhatri$ }git add Jenkinsfile
bash: }git: command not found
(base) rajnishatrismbp:pipeline rajnishkhatri$ git add Jenkinsfile
(base) rajnishatrismbp:pipeline rajnishkhatri$ git commit -m "commit for pipelin repo again"
[main 411152c] commit for pipelin repo again
 1 file changed, 7 insertions(+), 18 deletions(-)
(base) rajnishatrismbp:pipeline rajnishkhatri$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 465 bytes | 465.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/NeetuSDET/Pipeline_Practice.git
   d836541..411152c  main -> main
(base) rajnishatrismbp:pipeline rajnishkhatri$ 
