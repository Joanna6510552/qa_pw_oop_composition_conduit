# OOP & Composition for Conduit Test Project

## Table of Contents

- [Description](#description)
- [Preparation](#preparation)
- [Main Task](#main-task)
- [Task Reporting](#task-reporting)

## Description

In this task, you'll practice creating reusable components and using Object-Oriented Programming (OOP). 
You'll create components for:

- Conduit `ExternalHomePage`:

![external home page](https://github.com/mate-academy/qa_pw_oop_composition_conduit/blob/main/ExternalHome.png) 

- `InternalHomePage`:

![internal home page](https://github.com/mate-academy/qa_pw_oop_composition_conduit/blob/main/InternalHome.png) 

- `ExternalViewArticlePage`:

![external view article page](https://github.com/mate-academy/qa_pw_oop_composition_conduit/blob/main/ExternalViewArticlePage.png) 

- `InternalViewArticlePage`:

![internal view article page](https://github.com/mate-academy/qa_pw_oop_composition_conduit/blob/main/InternalViewArticlePage.png) 

## Preparation

1. Open the forked repo in VSCode.
2. Create a new branch by running `git checkout -b task_solution`.
3. Run the installation commands:

    - `npm ci`
    - `npx playwright install`

## Main Task

1. Write new tests for the [Conduit](https://conduit.mate.academy/) site: 
- A logged-in user can view their own article in the **Global Feed** section.
- A logged-in user can find their own article by tag from the **Popular Tags** section and view it in the **Tag Feed**.
- A non-logged-in user can view articles created by other users in the **Global Feed** section.
- A non-logged-in user can open an article page created by other users from the **Global Feed** section.

2. To write these tests, work with the components and base pages:
* 2.1 
- Create a component named `PopularTags`.
- Initialize the `PopularTags` component in the `BaseHomePage` class.
* 2.2 
- Create a component named `ArticleListItem`.
- Initialize the `ArticleFeedItem` component in the `Popular Feeds` class.
- Initialize the `ArticleFeedItem` component in the `Global Feeds` class.
* 2.3
- Create a component named `TagFeed`.
- Initialize the `TagFeed` component in the `ExternalHomePage`.
- Initialize the `TagFeed` component in the `InternalHomePage`.
* 2.4
- Create a page named `BaseViewArticlePage`.
- Extend the `ExternalViewArticlePage` and `InternalViewArticlePage` pages from the `BaseViewArticlePage`.
* 2.5
- Create a component named `BaseViewArticleBlock`.
- Extend the `ExternalViewArticleBlock` and `InternalViewArticleBlock` from the `BaseViewArticleBlock` component.
- Initialize the `InternalViewArticleBlock` component within the `InternalViewArticlePage` constructor.
- Initialize the `ExternalViewArticleBlock` component within the `ExternalViewArticlePage` constructor.
3. Run all tests and make sure they pass.

## Task Reporting

1. Add and commit all your updates.
2. Push the code to the origin.
3. Create a PR for your changes.
4. Keep implementing suggestions from the code review until your PR is approved.
