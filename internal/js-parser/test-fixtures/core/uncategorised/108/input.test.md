# `index.test.ts`

**DO NOT MODIFY**. This file has been autogenerated. Run `rome test internal/js-parser/index.test.ts --update-snapshots` to update.

## `core > uncategorised > 108`

### `ast`

```javascript
JSRoot {
	comments: Array []
	corrupt: false
	directives: Array []
	filename: "core/uncategorised/108/input.js"
	hasHoistedVars: true
	interpreter: undefined
	mtime: undefined
	sourceType: "script"
	syntax: Array []
	loc: Object {
		filename: "core/uncategorised/108/input.js"
		end: Object {
			column: 22
			line: 1
		}
		start: Object {
			column: 0
			line: 1
		}
	}
	diagnostics: Array [
		Object {
			origins: Array [Object {category: "parse/js"}]
			description: Object {
				advice: Array []
				category: "parse/js"
				message: MARKUP {parts: Array [RAW_MARKUP {value: "Regular expression flags can't contain unicode escapes"}]}
			}
			location: Object {
				filename: "core/uncategorised/108/input.js"
				mtime: undefined
				sourceText: undefined
				end: Object {
					column: 16
					line: 1
				}
				start: Object {
					column: 16
					line: 1
				}
			}
		}
	]
	body: Array [
		JSVariableDeclarationStatement {
			loc: Object {
				filename: "core/uncategorised/108/input.js"
				end: Object {
					column: 22
					line: 1
				}
				start: Object {
					column: 0
					line: 1
				}
			}
			declaration: JSVariableDeclaration {
				kind: "var"
				loc: Object {
					filename: "core/uncategorised/108/input.js"
					end: Object {
						column: 22
						line: 1
					}
					start: Object {
						column: 0
						line: 1
					}
				}
				declarations: Array [
					JSVariableDeclarator {
						id: JSBindingIdentifier {
							name: "x"
							loc: Object {
								filename: "core/uncategorised/108/input.js"
								identifierName: "x"
								end: Object {
									column: 5
									line: 1
								}
								start: Object {
									column: 4
									line: 1
								}
							}
						}
						loc: Object {
							filename: "core/uncategorised/108/input.js"
							end: Object {
								column: 22
								line: 1
							}
							start: Object {
								column: 4
								line: 1
							}
						}
						init: JSRegExpLiteral {
							global: true
							insensitive: false
							multiline: false
							noDotNewline: false
							sticky: false
							unicode: false
							loc: Object {
								filename: "core/uncategorised/108/input.js"
								end: Object {
									column: 22
									line: 1
								}
								start: Object {
									column: 8
									line: 1
								}
							}
							expression: JSRegExpSubExpression {
								loc: Object {
									filename: "core/uncategorised/108/input.js"
									end: Object {
										column: 14
										line: 1
									}
									start: Object {
										column: 9
										line: 1
									}
								}
								body: Array [
									JSRegExpCharSet {
										invert: false
										loc: Object {
											filename: "core/uncategorised/108/input.js"
											end: Object {
												column: 14
												line: 1
											}
											start: Object {
												column: 9
												line: 1
											}
										}
										body: Array [
											JSRegExpCharacter {
												value: "P"
												loc: Object {
													filename: "core/uncategorised/108/input.js"
													end: Object {
														column: 11
														line: 1
													}
													start: Object {
														column: 10
														line: 1
													}
												}
											}
											JSRegExpCharacter {
												value: " "
												loc: Object {
													filename: "core/uncategorised/108/input.js"
													end: Object {
														column: 12
														line: 1
													}
													start: Object {
														column: 11
														line: 1
													}
												}
											}
											JSRegExpCharacter {
												value: "Q"
												loc: Object {
													filename: "core/uncategorised/108/input.js"
													end: Object {
														column: 13
														line: 1
													}
													start: Object {
														column: 12
														line: 1
													}
												}
											}
											JSRegExpCharacter {
												value: "R"
												loc: Object {
													filename: "core/uncategorised/108/input.js"
													end: Object {
														column: 14
														line: 1
													}
													start: Object {
														column: 13
														line: 1
													}
												}
											}
										]
									}
								]
							}
						}
					}
				]
			}
		}
	]
}
```

### `diagnostics`

```

 core/uncategorised/108/input.js:1:16 parse/js ━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  ✖ Regular expression flags can't contain unicode escapes

    var x = /[P QR]/\u0067
                    ^

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

✖ Found 1 problem

```
