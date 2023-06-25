# codepath-onboarding-graphql
GraphQL query for a Codepath onboarding assignment.

query codePathOnboardingAssignment {
  allSpecies {
    totalCount
    species {
      ...heightAndLifespan
    }
  }
}

fragment heightAndLifespan on Species {
  averageHeight
  averageLifespan
}
