# SRMP 2026: Planets with Gaia

Notebooks for our Science Research Mentoring Program group. This year we are getting ready for Gaia Data Release 4 (out December 2026), which should contain thousands of new planet candidates found by watching stars wobble. Our job is to predict what it will find, then check.

## How to run the notebooks

You don't need to install anything. Pick one:

**Option 1: GitHub Codespaces (runs inside GitHub)**

1. Click the green **Code** button at the top of this page.
2. Choose the **Codespaces** tab, then **Create codespace on main**.
3. Wait a minute or two while it sets up. A VS Code window opens in your browser.
4. Open the `notebooks` folder on the left and click a notebook. When asked for a kernel, pick **Python 3.11**.

Your codespace is saved to your GitHub account, so your work is still there next week.

**Option 2: Google Colab**

Click the badge next to a notebook below. Colab opens it in your Google account. Use **File → Save a copy in Drive** so your edits stick.

## Notebooks

| Session | Notebook | Open in Colab |
|---|---|---|
| 4 | [The planet zoo, in Python](notebooks/Session4_PlanetZoo.ipynb) | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/jeaadams/srmp-gaia-planets/blob/main/notebooks/Session4_PlanetZoo.ipynb) |

## Data

The notebooks load the [NASA Exoplanet Archive](https://exoplanetarchive.ipac.caltech.edu) Planetary Systems Composite table live over the internet. If the archive is down, `data/planetary_systems_2026-11-22.csv` is a snapshot you can load instead:

```python
df = pd.read_csv("../data/planetary_systems_2026-11-22.csv")
```

## Reading

- Lammers & Winn (2025), *On the Exoplanet Yield of Gaia Astrometry*, [arXiv:2511.04673](https://arxiv.org/abs/2511.04673)
- NASA Exoplanet Archive [Plotting Tool](https://exoplanetarchive.ipac.caltech.edu/exoplanetplots/)
