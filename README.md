---

# Forked Features: Clone Functionality

This fork adds support for cloning items between lists with the following options:

- **`clone: true`**  
  When set on the target list, allows items to be cloned (copied) rather than moved.

- **`locked: true`**  
  When set on the source list, prevents items from being transfered to.

### How it works

- The parent list is re-indexed on each insert to maintain order.
- Each item in the source list **must have a unique `key`** upfront, which is used for indexing.
- Enables flexible drag-and-drop behavior where the source list acts as a locked palette, and the target list receives clones of those items.

---
Only tested in vue
Feel free to reach out if you have questions or want to contribute back!
## Install

```bash 
npm install formkit-clone-feature
```

You can also visit the package page here: https://www.npmjs.com/package/formkit-clone-feature