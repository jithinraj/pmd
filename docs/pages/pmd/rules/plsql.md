---
title: PLSQL Rules
permalink: pmd_rules_plsql.html
folder: pmd/rules
---
## Best Practices

{% include callout.html content="Rules which enforce generally accepted best practices." %}

*   [TomKytesDespair](pmd_rules_plsql_bestpractices.html#tomkytesdespair): "WHEN OTHERS THEN NULL" hides all errors - (Re)RAISE an exception or call RAISE_APPLICATION_ERROR

## Codestyle

{% include callout.html content="Rules which enforce a specific coding style." %}

*   [MisplacedPragma](pmd_rules_plsql_codestyle.html#misplacedpragma): Oracle states that the PRAQMA AUTONOMOUS_TRANSACTION must be in the declaration block,but the cod...

## Design

{% include callout.html content="Rules that help you discover design issues." %}

*   [CyclomaticComplexity](pmd_rules_plsql_design.html#cyclomaticcomplexity): Complexity directly affects maintenance costs is determined by the number of decision points in a...
*   [ExcessiveMethodLength](pmd_rules_plsql_design.html#excessivemethodlength): When methods are excessively long this usually indicates that the method is doing more than itsna...
*   [ExcessiveObjectLength](pmd_rules_plsql_design.html#excessiveobjectlength): Excessive object line lengths are usually indications that the object may be burdened with excess...
*   [ExcessivePackageBodyLength](pmd_rules_plsql_design.html#excessivepackagebodylength): Excessive class file lengths are usually indications that the class may be burdened with excessiv...
*   [ExcessivePackageSpecificationLength](pmd_rules_plsql_design.html#excessivepackagespecificationlength): Excessive class file lengths are usually indications that the class may be burdened with excessiv...
*   [ExcessiveParameterList](pmd_rules_plsql_design.html#excessiveparameterlist): Methods with numerous parameters are a challenge to maintain, especially if most of them share th...
*   [ExcessiveTypeLength](pmd_rules_plsql_design.html#excessivetypelength): Excessive class file lengths are usually indications that the class may be burdened with excessiv...
*   [NcssMethodCount](pmd_rules_plsql_design.html#ncssmethodcount): This rule uses the NCSS (Non-Commenting Source Statements) algorithm to determine the number of l...
*   [NcssObjectCount](pmd_rules_plsql_design.html#ncssobjectcount): This rule uses the NCSS (Non-Commenting Source Statements) algorithm to determine the number of l...
*   [NPathComplexity](pmd_rules_plsql_design.html#npathcomplexity): The NPath complexity of a method is the number of acyclic execution paths through that method.A t...
*   [TooManyFields](pmd_rules_plsql_design.html#toomanyfields): Classes that have too many fields can become unwieldy and could be redesigned to have fewer field...
*   [TooManyMethods](pmd_rules_plsql_design.html#toomanymethods): A package or type with too many methods is probably a good suspect for refactoring, in order to r...

## Error Prone

{% include callout.html content="Rules to detect constructs that are either broken, extremely confusing or prone to runtime errors." %}

*   [TO_DATE_TO_CHAR](pmd_rules_plsql_errorprone.html#to_date_to_char): TO_DATE(TO_CHAR(date-variable)) used to remove time component - use TRUNC(date-variable)
*   [TO_DATEWithoutDateFormat](pmd_rules_plsql_errorprone.html#to_datewithoutdateformat): TO_DATE without date format- use TO_DATE(expression, date-format)
*   [TO_TIMESTAMPWithoutDateFormat](pmd_rules_plsql_errorprone.html#to_timestampwithoutdateformat): TO_TIMESTAMP without date format- use TO_TIMESTAMP(expression, date-format)

## Additional rulesets

*   Code Size (`rulesets/plsql/codesize.xml`):

    <span style="border-radius: 0.25em; color: #fff; padding: 0.2em 0.6em 0.3em; display: inline; background-color: #d9534f; font-size: 75%;">Deprecated</span>  This ruleset is for backwards compatibility.

    It contains the following rules:

    [CyclomaticComplexity](pmd_rules_plsql_design.html#cyclomaticcomplexity), [ExcessiveMethodLength](pmd_rules_plsql_design.html#excessivemethodlength), [ExcessiveObjectLength](pmd_rules_plsql_design.html#excessiveobjectlength), [ExcessivePackageBodyLength](pmd_rules_plsql_design.html#excessivepackagebodylength), [ExcessivePackageSpecificationLength](pmd_rules_plsql_design.html#excessivepackagespecificationlength), [ExcessiveParameterList](pmd_rules_plsql_design.html#excessiveparameterlist), [ExcessiveTypeLength](pmd_rules_plsql_design.html#excessivetypelength), [NcssMethodCount](pmd_rules_plsql_design.html#ncssmethodcount), [NcssObjectCount](pmd_rules_plsql_design.html#ncssobjectcount), [NPathComplexity](pmd_rules_plsql_design.html#npathcomplexity), [TooManyFields](pmd_rules_plsql_design.html#toomanyfields), [TooManyMethods](pmd_rules_plsql_design.html#toomanymethods)

*   PLSQL DATETIME (`rulesets/plsql/dates.xml`):

    <span style="border-radius: 0.25em; color: #fff; padding: 0.2em 0.6em 0.3em; display: inline; background-color: #d9534f; font-size: 75%;">Deprecated</span>  This ruleset is for backwards compatibility.

    It contains the following rules:

    [TO_DATE_TO_CHAR](pmd_rules_plsql_errorprone.html#to_date_to_char), [TO_DATEWithoutDateFormat](pmd_rules_plsql_errorprone.html#to_datewithoutdateformat), [TO_TIMESTAMPWithoutDateFormat](pmd_rules_plsql_errorprone.html#to_timestampwithoutdateformat)

*   Strict Syntax (`rulesets/plsql/strictsyntax.xml`):

    <span style="border-radius: 0.25em; color: #fff; padding: 0.2em 0.6em 0.3em; display: inline; background-color: #d9534f; font-size: 75%;">Deprecated</span>  This ruleset is for backwards compatibility.

    It contains the following rules:

    [MisplacedPragma](pmd_rules_plsql_codestyle.html#misplacedpragma)

*   Tom Kyte's Despair (`rulesets/plsql/TomKytesDespair.xml`):

    <span style="border-radius: 0.25em; color: #fff; padding: 0.2em 0.6em 0.3em; display: inline; background-color: #d9534f; font-size: 75%;">Deprecated</span>  This ruleset is for backwards compatibility.

    It contains the following rules:

    [TomKytesDespair](pmd_rules_plsql_bestpractices.html#tomkytesdespair)


