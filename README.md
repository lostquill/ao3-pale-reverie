## Installing the "My Pastel Default" skin

The skin works in layers: you need to create all three skins **in order** — the two parents first, then the main skin that brings them together.

> [!NOTE]
> The order of the parent skins is not critical here since the two don't overlap (one targets `all`, the other is limited to mobile/tablet). If you notice any conflict, add `My Default` first.

---

### Step 1 — Create `My Default`

1. Go to AO3 and log in
2. Click your username → **My Preferences** → **Skins**
3. Click **Create Site Skin**
4. Fill in the following fields:

| Field | Value |
|-------|-------|
| Title | `My Default LQ` |
| CSS | *(paste the contents of `default.css`)* |

5. Under **Advanced**, set:

| Field | Value |
|-------|-------|
| What it does | `add on to archive skin` |
| Media | `all` |

6. Click **Submit**

---

### Step 2 — Create `My Default - Mobile/Tablet`

1. Still in Skins → **Create Site Skin**
2. Fill in the following fields:

| Field | Value |
|-------|-------|
| Title | `My Default - Mobile/Tablet` |
| CSS | *(paste the contents of `mobile-tablet.css`)* |

3. Under **Advanced**, set:

| Field | Value |
|-------|-------|
| What it does | `add on to archive skin` |
| Media | `only screen and (max-width: 62em)` |

4. Click **Submit**

---

### Step 3 — Create `My Pastel Default`

This is the main skin — the one you will actually activate.

1. Still in Skins → **Create Site Skin**
2. Fill in the following fields:

| Field | Value |
|-------|-------|
| Title | `My Pastel Default` |
| CSS | `.test { opacity: 1; }` |

3. Under **Advanced**, set:

| Field | Value |
|-------|-------|
| What it does | `add on to archive skin` |
| Media | `all` |

4. Under **Parent Skins**, click **Add parent skin** twice and select:
   - `My Default LQ`
   - `My Default - Mobile/Tablet`

5. Click **Submit**

---

### Step 4 — Activate the skin

1. Go to **My Preferences**
2. Under **Site skin**, find `My Pastel Default`
3. Click **Use** next to it
4. Save your preferences
