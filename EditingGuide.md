# Guide to Editing - One-Among.Us

Other languages: [简体中文](EditingGuide-zh_Hans.md)

## Principles of Writing

We aim to be a small memorial rather than a wiki. Therefore, we encourage you to write to mourn those transgender friends or allies who have passed away, and to soothe those who are still alive. No matter what gender identity they were, we hope to show our readers, “they were the same as me. They are one among us.” Therefore, both overly exaggerated or overly calm descriptions need to be avoided.

You have more creative freedom than contributing to a wiki, but you should still follow some fundamental principles, such as:
- Be as truthful as possible.
- For large paragraphs of quotations, the source needs to be indicated.
- Slangs in the community can be used, but if you like, please add a comment when they first appear.

The article should be written in third person. Please use proper gender pronouns in accordance with the wishes of them. For non-binary, agender or gender-non-confirming people, if they did not show their pronouns, please use “they” in English and「ta」in Chinese for there is no proper, common Chinese characters at present. Or you can use your language skills to avoid pronouns.

Use proper punctuations in articles. In Chinese articles, regardless of different Chinese variants, use「」(outer) and『』(inner) for quotation marks in replace of “” or ‘’ unless the words in the quotation marks are not Chinese. Use curly quotation marks instead of straight ones.

If referring to outside resources, use web archive services such as [Internet Archive](https://archive.org) and [archive.today](https://archive.ph) (see [data/#141](https://github.com/one-among-us/data/issues/141)). 

To protect our readers, if someone departed from us through suicide, please hide the detail of their methods as you can. You must not write down the name or dose of the medicine or drugs if it was an overdose or poisoning.

To respect the privacy of the departed, unless we get specific authorization before they leave, we should not connect their different internet identities (just pick the most public one) or publish messages they have posted on private or anonymous SNS platforms. 

## Contribute with GitHub

Before proceeding, you may assure yourself that you have knowledge of:
- basics of `git`: cloning repositories, making commits, rebasing a branch to the main branch, and syncing between upstream and local repositories;
- basics of GitHub: forking repositories, creating pull requests, and collaborate with other GitHub users;
- basic grammar of the YAML language: indentation rules, usage of dash, spaces, and quotes, and escaping from special characters;
- basic grammar of the Markdown language.

Otherwise, you can simply email your writings and advices to [info@one-among.us](mailto:info@one-among.us). Our staff will transform them to the proper format. We do not assume our contributors have to master any technical skills – at any time, you can work in a more “traditional” way and your contribution will also be highly recognized.

## Supported features

### Comments

Not only the HTML comment `<!--` and `-->` but also the JSX comment `{/*` and `*/}` could be used as comment block. For example:

``` HTML
<!-- This is a comment, won't shown on tha page. -->
```

``` JSX
{/* This is also a comment and will not be displayed in the page */}
```

### Icons embedded in pages

Supports inline icons similar to `[!Note]`. As of this writing (Apr.7, 2024), supported icons are as shown in the following table:  

|Tag|Icon|
|:-:|:-:|
|`[!Caution]`|<svg style="display: inline-block; overflow: visible !important; vertical-align: sub; fill: rgb(209, 36, 47); margin-right: 10px;" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M4.47.22A.749.749 0 0 1 5 0h6c.199 0 .389.079.53.22l4.25 4.25c.141.14.22.331.22.53v6a.749.749 0 0 1-.22.53l-4.25 4.25A.749.749 0 0 1 11 16H5a.749.749 0 0 1-.53-.22L.22 11.53A.749.749 0 0 1 0 11V5c0-.199.079-.389.22-.53Zm.84 1.28L1.5 5.31v5.38l3.81 3.81h5.38l3.81-3.81V5.31L10.69 1.5ZM8 4a.75.75 0 0 1 .75.75v3.5a.75.75 0 0 1-1.5 0v-3.5A.75.75 0 0 1 8 4Zm0 8a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"></path></svg>|
|`[!Warning]`|<svg style="display: inline-block; overflow: visible !important; vertical-align: sub; fill: rgb(154, 103, 0); margin-right: 10px;" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M6.457 1.047c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0 1 14.082 15H1.918a1.75 1.75 0 0 1-1.543-2.575Zm1.763.707a.25.25 0 0 0-.44 0L1.698 13.132a.25.25 0 0 0 .22.368h12.164a.25.25 0 0 0 .22-.368Zm.53 3.996v2.5a.75.75 0 0 1-1.5 0v-2.5a.75.75 0 0 1 1.5 0ZM9 11a1 1 0 1 1-2 0 1 1 0 0 1 2 0Z"></path></svg>|
|`[!Important]`|<svg style="display: inline-block; overflow: visible !important; vertical-align: sub; fill: rgb(130, 80, 223); margin-right: 10px;" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M0 1.75C0 .784.784 0 1.75 0h12.5C15.216 0 16 .784 16 1.75v9.5A1.75 1.75 0 0 1 14.25 13H8.06l-2.573 2.573A1.458 1.458 0 0 1 3 14.543V13H1.75A1.75 1.75 0 0 1 0 11.25Zm1.75-.25a.25.25 0 0 0-.25.25v9.5c0 .138.112.25.25.25h2a.75.75 0 0 1 .75.75v2.19l2.72-2.72a.749.749 0 0 1 .53-.22h6.5a.25.25 0 0 0 .25-.25v-9.5a.25.25 0 0 0-.25-.25Zm7 2.25v2.5a.75.75 0 0 1-1.5 0v-2.5a.75.75 0 0 1 1.5 0ZM9 9a1 1 0 1 1-2 0 1 1 0 0 1 2 0Z"></path></svg>|
|`[!Tip]`|<svg style="display: inline-block; overflow: visible !important; vertical-align: sub; fill: rgb(26, 127, 55); margin-right: 10px;" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M8 1.5c-2.363 0-4 1.69-4 3.75 0 .984.424 1.625.984 2.304l.214.253c.223.264.47.556.673.848.284.411.537.896.621 1.49a.75.75 0 0 1-1.484.211c-.04-.282-.163-.547-.37-.847a8.456 8.456 0 0 0-.542-.68c-.084-.1-.173-.205-.268-.32C3.201 7.75 2.5 6.766 2.5 5.25 2.5 2.31 4.863 0 8 0s5.5 2.31 5.5 5.25c0 1.516-.701 2.5-1.328 3.259-.095.115-.184.22-.268.319-.207.245-.383.453-.541.681-.208.3-.33.565-.37.847a.751.751 0 0 1-1.485-.212c.084-.593.337-1.078.621-1.489.203-.292.45-.584.673-.848.075-.088.147-.173.213-.253.561-.679.985-1.32.985-2.304 0-2.06-1.637-3.75-4-3.75ZM5.75 12h4.5a.75.75 0 0 1 0 1.5h-4.5a.75.75 0 0 1 0-1.5ZM6 15.25a.75.75 0 0 1 .75-.75h2.5a.75.75 0 0 1 0 1.5h-2.5a.75.75 0 0 1-.75-.75Z"></path></svg>|
|`[!Note]`|<svg style="display: inline-block; overflow: visible !important; vertical-align: sub; fill: rgb(9, 105, 218); margin-right: 10px;" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="M0 8a8 8 0 1 1 16 0A8 8 0 0 1 0 8Zm8-6.5a6.5 6.5 0 1 0 0 13 6.5 6.5 0 0 0 0-13ZM6.5 7.75A.75.75 0 0 1 7.25 7h1a.75.75 0 0 1 .75.75v2.75h.25a.75.75 0 0 1 0 1.5h-2a.75.75 0 0 1 0-1.5h.25v-2h-.25a.75.75 0 0 1-.75-.75ZM8 6a1 1 0 1 1 0-2 1 1 0 0 1 0 2Z"></path></svg>|
|`[!Alert]`|<svg style="display: inline-block; overflow: visible !important; vertical-align: sub; fill: #ff7800; margin-right: 10px;" viewBox="0 0 20 20" version="1.1" width="16" height="16" aria-hidden="true"><path d="M12 2c-.5 0-1 .19-1.41.59l-8 8c-.79.78-.79 2.04 0 2.82l8 8c.78.79 2.04.79 2.82 0l8-8c.79-.78.79-2.04 0-2.82l-8-8C13 2.19 12.5 2 12 2m0 2l8 8l-8 8l-8-8m7-5v6h2V7m-2 8v2h2v-2Z"/></svg>|
|`[!Annotation]`|<svg style="display: inline-block; overflow: visible !important; vertical-align: sub; fill: #865e3c; margin-right: 10px;" viewBox="0 0 20 20" version="1.1" width="16" height="16" aria-hidden="true"><path d="M12 15c.81 0 1.5-.3 2.11-.89c.59-.61.89-1.3.89-2.11c0-.81-.3-1.5-.89-2.11C13.5 9.3 12.81 9 12 9c-.81 0-1.5.3-2.11.89C9.3 10.5 9 11.19 9 12c0 .81.3 1.5.89 2.11c.61.59 1.3.89 2.11.89m0-13c2.75 0 5.1 1 7.05 2.95C21 6.9 22 9.25 22 12v1.45c0 1-.35 1.85-1 2.55c-.7.67-1.5 1-2.5 1c-1.2 0-2.19-.5-2.94-1.5c-1 1-2.18 1.5-3.56 1.5c-1.37 0-2.55-.5-3.54-1.46C7.5 14.55 7 13.38 7 12c0-1.37.5-2.55 1.46-3.54C9.45 7.5 10.63 7 12 7c1.38 0 2.55.5 3.54 1.46C16.5 9.45 17 10.63 17 12v1.45c0 .41.16.77.46 1.08c.3.31.65.47 1.04.47c.42 0 .77-.16 1.07-.47c.3-.31.43-.67.43-1.08V12c0-2.19-.77-4.07-2.35-5.65S14.19 4 12 4c-2.19 0-4.07.77-5.65 2.35S4 9.81 4 12c0 2.19.77 4.07 2.35 5.65S9.81 20 12 20h5v2h-5c-2.75 0-5.1-1-7.05-2.95C3 17.1 2 14.75 2 12s1-5.1 2.95-7.05C6.9 3 9.25 2 12 2"/></svg>|
|`[!TransFlag]`|<svg style="display: inline-block; overflow: visible !important; vertical-align: sub; margin-right: 10px;" viewBox="0 0 32 32" width="16" height="16" aria-hidden="true"><path fill="#5BCEFA" d="M0 27c0 2.209 1.791 4 4 4h28c2.209 0 4-1.791 4-4v-1.3H0V27z"/><path fill="#F5A9B8" d="M.026 20.5L0 25.8h36v-5.3z"/><path fill="#EEE" d="M0 15.3h36v5.3H0z"/><path fill="#F5A9B8" d="M0 9.902h36V15.4H0z"/><path fill="#5BCEFA" d="M36 9c0-2.209-1.791-4-4-4H4C1.791 5 0 6.791 0 9v1.2h36V9z"/></svg>|
|`[!Pride]`|<svg style="display: inline-block; overflow: visible !important; vertical-align: sub; margin-right: 10px;" viewBox="0 0 32 32" width="16" height="16" aria-hidden="true"><path fill="#880082" d="M0 27a4 4 0 0 0 4 4h28a4 4 0 0 0 4-4v-.5H0v.5z"/><path fill="#3558A0" d="M0 22.07h36v4.6H0z"/><path fill="#138F3E" d="M0 17.83h36v4.5H0z"/><path fill="#FAD220" d="M0 13.5h36V18H0z"/><path fill="#FF7300" d="M0 9.17h36v4.5H0z"/><path fill="#FF000E" d="M32 5H4a4 4 0 0 0-4 4v.33h36V9a4 4 0 0 0-4-4z"/></svg>|

*Under construction*

