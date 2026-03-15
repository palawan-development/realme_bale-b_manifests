# realme GT Neo6 manifests

### How to use

**Create ROM directory and initialize it's repository (if you haven't done that yet)**
```bash
mkdir -p LineageOS; cd LineageOS
repo init \
-u https://github.com/LineageOS/android.git \
-b lineage-<version> \
--git-lfs
```

**Clone your manifest**
```bash
git clone https://github.com/palawan-development/realme_baleb_manifests.git .repo/local_manifests
-b <specified-branch>
```

**Sync**
```bash
repo sync \
--no-clone-bundle -c -n --prune --force-sync --optimized-fetch --no-tags \
--retry-fetches=5 \
-j<specified-number-of-jobs>
```

**Done! All repositories from the manifest should be synchronized**
