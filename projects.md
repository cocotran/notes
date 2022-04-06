## Angular

#### Characters limit and patterns (pattern, text, input)
```html
<mat-form-field
  color="primary"
  [hintLabel]="(rulenameInputField.focused ? 'GENERAL.MAX_N_CHARACTERS' : '') | translate: { value: 100 }"
>
  <input
    [(ngModel)]="prefixRule.GROUPNAME"
    (blur)="updatePrefixRuleName(prefixRule.GROUPNAME)"
    name="name"
    type="text"
    required
    placeholder="{{ 'GENERAL.NAME' | translate }}"
    matInput
    #rulenameInputField="matInput"
    maxlength="100"
    #rulenameInput="ngModel"
    pattern="[a-zA-Z0-9_-]{0,100}"
  />
  <mat-error
    [style.visibility]="rulenameInput.errors?.pattern ? 'visible' : 'hidden'"
    style="font-size: 12px"
    >{{ 'GENERAL.CHARACTER_NOT_VALID' | translate }}</mat-error
  >
  <mat-hint
    *ngIf="rulenameInputField.focused && !rulenameInputField.errors"
    align="end"
    >{{ rulenameInputField.value?.length || 0 }}/100</mat-hint
  >
</mat-form-field>
```

---


## CSS

#### Add ellipsis to text (text, input)
```
.ellipsis {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
}
```

---

## Git

#### Git squash
```bash
git reset --soft <commit>
git commit -m "new commit"
git push -f
````

---

## HTML

#### Set fixed width for table column (table, cell)
```html
<table class="text-center" style="table-layout: fixed; width: 100%">
  <col style="width: 200px" />
  <col style="width: 50%" />
</table>
```