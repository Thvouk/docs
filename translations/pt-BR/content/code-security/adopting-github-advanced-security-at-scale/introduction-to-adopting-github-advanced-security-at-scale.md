---
title: Introduction to adopting GitHub Advanced Security at scale
intro: 'You can adopt {% data variables.product.prodname_GH_advanced_security %} at scale in your company following industry and GitHub best practices.'
versions:
  ghes: '*'
  ghae: '*'
  ghec: '*'
topics:
  - Advanced Security
shortTitle: Introdução
redirect_from:
  - /admin/advanced-security/overview-of-github-advanced-security-deployment
  - /admin/code-security/managing-github-advanced-security-for-your-enterprise/overview-of-github-advanced-security-deployment
  - /admin/advanced-security/deploying-github-advanced-security-in-your-enterprise
  - /admin/code-security/managing-github-advanced-security-for-your-enterprise/deploying-github-advanced-security-in-your-enterprise
miniTocMaxHeadingLevel: 2
---

## About these articles

{% data variables.product.prodname_GH_advanced_security %} (GHAS) helps teams build more secure code faster using integrated tooling such as secret scanning and code scanning using CodeQL. To understand the security features available through {% data variables.product.prodname_GH_advanced_security %}, see "[About GitHub Advanced Security](/get-started/learning-about-github/about-github-advanced-security)."

O GHAS é um conjunto de ferramentas que requer a participação ativa de desenvolvedores na sua empresa. To realize the best return on your investment, you must learn how to use, apply, and maintain GHAS.


Criamos uma abordagem faseada para implementações do GHAS desenvolvidas com base nas práticas recomendadas do setor e do GitHub. We expect most customers will want to follow these phases, based on our experience helping customers with a successful deployment of {% data variables.product.prodname_GH_advanced_security %}, but you may need to modify this approach to meet the needs of your company.

Enabling GHAS across a large organization can be broken down into six core phases.

1. [**Align on your rollout strategy and goals**](/code-security/adopting-github-advanced-security-at-scale/phase-1-align-on-your-rollout-strategy-and-goals): Think about what success will look like, and align on how GHAS will be implemented in your company. This phase may only take a few days or a week, but it lays a solid foundation for the rest of the rollout.

2. [**Preparing to enable at scale**](/code-security/adopting-github-advanced-security-at-scale/phase-2-preparing-to-enable-at-scale): Prepare developers, collect data about your repositories, and ensure you're ready for the next phase.

3. [**Pilot programs**](/code-security/adopting-github-advanced-security-at-scale/phase-3-pilot-programs): Optionally, pilot an initial rollout to a few high-impact projects and teams. This will allow an initial group within your company to get familiar with GHAS before you roll out to the remainder of your company.

4. [**Create internal documentation**](/code-security/adopting-github-advanced-security-at-scale/phase-4-create-internal-documentation): Create and communicate internal documentation for the consumers of GHAS. Without proper documentation provided to developers, security engineers, and others who will be using GHAS, the value will get lost in the rollout.

5. [**Rollout and scale {% data variables.product.prodname_code_scanning %}**](/code-security/adopting-github-advanced-security-at-scale/phase-5-rollout-and-scale-code-scanning): Leveraging the available APIs, automatically rollout {% data variables.product.prodname_code_scanning %} by team and by language across your enterprise, using the repository data you collected earlier.

6. [**Rollout and scale {% data variables.product.prodname_secret_scanning %}**](/code-security/adopting-github-advanced-security-at-scale/phase-6-rollout-and-scale-secret-scanning): Roll out {% data variables.product.prodname_secret_scanning %}, which involves less configuration and is therefore simpler to adopt than {% data variables.product.prodname_code_scanning %}. Still, it's critical to have a strategy for handling new and old results.

## {% data variables.contact.github_support %} e {% data variables.product.prodname_professional_services_team %}

If you encounter any issues or have any questions during your implementation, you can search our documentation for solutions or engage with {% data variables.contact.github_support %}. Para obter mais informações, consulte "[Sobre GitHub Support](/support/learning-about-github-support/about-github-support)".

If you prefer to have guidance throughout the rollout process, {% data variables.product.prodname_professional_services %} can partner with you for a successful rollout and implementation of {% data variables.product.prodname_GH_advanced_security %}. We offer a variety of options for guidance and support. We also have training and bootcamps available to help your company to optimize the value of {% data variables.product.prodname_GH_advanced_security %}.

Speak with your sales representative for more information about all the Professional Services options available. Para mais informações, entre em contato com {% data variables.contact.contact_enterprise_sales %}.

{% note %}

For the first article in this series, see "[Phase 1: Align on your rollout strategy and goals](/code-security/adopting-github-advanced-security-at-scale/phase-1-align-on-your-rollout-strategy-and-goals)."

{% endnote %}
