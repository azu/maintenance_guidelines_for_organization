# Organizationのためのメンテナンスガイドライン

このガイドラインは[[GITHUB_ORGANIZATION_NAME]] organizationの既存、新しいメンバーに対するものです。

このドキュメントは新しいメンバーやパッケージを追加する手順についてを紹介しています。

## 原則

- 人がボトルネックになることを避けること
- 人が正しいことをできるように信用すること(正しくないことが証明されない限り)

人がボトルネックになるのを避けるためには、すべてのメンバーがプロジェクト管理に必要な権限を扱える必要があります。

いくつかの行動については他のメンバーやコミュニティと適切であるかを話し合ったほうが良いかもしれません。その他については個人の決定を優先して良いでしょう。

不適切な行動についてはプロジェクトチームの [[INSERT_EMAIL_ADDRESS]] に報告されるかもしれません。
不適切な行動は [Code of Conduct][] に定義されています。

すべての苦情は、レビュー、調査され、必要かつ適切と判断された対応がとられます。プロジェクトチームは、事象の報告者に関する守秘義務があります。

## For maintainer

メンテナーは自由に新しいメンバーを追加できます。

[Code of Conduct][] に同意でき、プロジェクトに関心がある信用できる人を見つけた場合、次の手順でプロジェクトのメンバーに追加できます。

### GitHub

1. [https://github.com/orgs/[[GITHUB_ORGANIZATION_NAME]]/people](https://github.com/orgs/[[GITHUB_ORGANIZATION_NAME]]/people) を開く
2. **Invite member**をクリック
3. 招待したいメンバーのユーザ名またはEmailを入力
4. "**Owner**"を選択
5. Send Invitationする

詳細は [Inviting users to join your organization - User Documentation](https://help.github.com/articles/inviting-users-to-join-your-organization/) を参照してください。

### npm

1. [https://www.npmjs.com/settings/[[NPM_ORGANIZATION_NAME]]/members](https://www.npmjs.com/settings/[[NPM_ORGANIZATION_NAME]]/members)を開く
2. 招待したいメンバーのユーザ名またはEmailを入力
3. "**Owner**"を選択
4. **add member**をクリック

詳細は [Managing Members · npm Orgs Documentation](https://www.npmjs.com/docs/orgs/managing-members.html) を参照してください。

## For new member

Organizationへパッケージを追加するには、次の手順で追加できます。

### GitHub

Organizationへパッケージを追加するには、次の手順で追加できます。

1. [https://github.com/$USER/$PROJECT/settings](https://github.com/%24USER/%24PROJECT/settings) (リポジトリの設定ページ) を開く
2. **Transfer** をクリック
3. "New owner's GitHub username or organization name"に[[GITHUB_ORGANIZATION_NAME]] と入力
4. "I understand, transfer this repository" をクリックして移譲

詳細は [About repository transfers - User Documentation](https://help.github.com/articles/about-repository-transfers/) を参照してください。

### npm

次のコマンドの `$PKGNAME` を自分のパッケージ名に置き換えてから実行してください。

```shell-session
npm access grant read-write [[NPM_ORGANIZATION_NAME]]:developers $PKGNAME
```

またはウェブ上でもパッケージの移譲が可能です。

1. <https://www.npmjs.com/settings/[[NPM_ORGANIZATION_NAME]]/teams/team/developers/access> を開く
2. "Package" に 移譲したいパッケージ名を入力
3. "Add Existing Packages"をクリックして移譲

詳細は次のページを参照してください。

- [Managing Package Access · npm Orgs Documentation](https://npm.github.io/orgs-docs/managing-package-access.html)

## Attribution

このガイドラインは [Maintenance Guidelines for Organization](https://maintenance-guidelines-for-organization.github.io/) に基づいています。

このガイドラインは Creative Commons Attribution 4.0 International Public License([CC BY 4.0](https://creativecommons.org/licenses/by/4.0/)) のライセンスで利用できます。

[Code of Conduct]: [[CODE_OF_CONDUCT_LINK]]