# Game Mechanics: Player Journey

---

## Player Journey Overview

The QuestPay™ player experience follows a carefully designed cycle that combines physical exploration, digital transactions, and competitive strategy.

---

## Sample Player Flow

### Step 1: Receive Initial QuestPay Code

**Delivery**: QR code or voucher link via:
- SMS
- Email  
- In-app notification
- Physical card (for special formats)

**Code Contains**:
- Unique identifier
- Encrypted challenge data
- Redemption instructions
- Time limits (if applicable)

### Step 2: Redeem via Partner Wallet

**Process**:

1. Contestant scans QR or clicks link
2. Partner wallet app opens automatically
3. Code validation occurs via x-Change API
4. Challenge instructions unlock
5. Starting funds (if any) credited to wallet

**Instructions Reveal**:
- Challenge location or merchant
- Transaction type required
- Success criteria
- Next step hints

### Step 3: Perform Mission Transaction

**Transaction Types**:

| Type | Example | Verification |
|------|---------|--------------|
| **Purchase** | Buy specific item from merchant | Receipt + API confirmation |
| **Bill Payment** | Pay utility or service bill | Payment reference number |
| **Donation** | Contribute to charity | NGO receipt + webhook |
| **Transfer** | Send money to someone | Transaction ID |
| **Top-Up** | Add load or credits | Confirmation code |

**Challenge Variations**:
- Simple: Single transaction at known location
- Moderate: Multiple steps or budget constraints
- Complex: Strategy required, multiple locations, time pressure

### Step 4: Verification via API Webhook

**Automatic Verification**:

```mermaid
sequenceDiagram
    Contestant->>Merchant: Makes Payment
    Merchant->>Wallet: Transaction Processed
    Wallet->>x-Change: Webhook Notification
    x-Change->>QuestPay Engine: Verify Challenge
    QuestPay Engine->>Leaderboard: Update Status
    QuestPay Engine->>Contestant: Release Next Code
```

**Verification Checks**:
- Correct merchant/recipient
- Correct amount (exact or within range)
- Completed within time limit
- Unique transaction (no duplicates)

### Step 5: Leaderboard Update

**Real-Time Updates**:
- Contestant position
- Time taken
- Points earned
- Next challengers behind them

**Broadcast Integration**:
- Live graphics on TV/stream
- Social media bot updates
- Mobile app notifications
- Physical leaderboard displays

### Step 6: Receive Next Quest Code

**Progressive Unlocking**:
- Next code delivered immediately upon verification
- Difficulty increases with each stage
- Final quest requires collecting all previous codes

---

## Real-Time Elements

### Live Dashboards

**For Contestants**:
- Current position and points
- Challenges completed vs. remaining
- Time elapsed
- Competitor proximity alerts

**For Viewers**:
- All contestant positions
- Transaction heat map
- Predicted winners
- Side quest opportunities

### Social Media Feeds

**Auto-Generated Content**:
- "Contestant X just completed challenge at Location Y!"
- Progress milestones and achievements
- Photo/video from challenge locations
- Viewer polls and predictions

### Public Leaderboards

**Display Locations**:
- Production studio
- Partner wallet apps
- QuestPay website
- Partner merchant screens
- Social media platforms

---

## Game Variations

### Speed Mode

**Objective**: Complete all challenges in fastest time

**Rules**:
- All contestants start simultaneously
- First to finish wins grand prize
- Time penalties for errors
- Bonus for perfect completion

### Points Accumulation

**Objective**: Earn maximum points across season

**Rules**:
- Points awarded based on completion time and difficulty
- Weekly challenges with varying point values
- Elimination of lowest scorers
- Grand finale for top contestants

### Team Relay

**Objective**: Team completes challenges cooperatively

**Rules**:
- 3-5 member teams
- Each member completes specific legs
- Handoff via code transfer
- Team coordination required

### Survival Format

**Objective**: Avoid elimination week by week

**Rules**:
- Weekly challenges
- Bottom performers face elimination
- Last person/team standing wins
- Alliances and strategy

---

## Challenge Difficulty Tiers

### Tier 1: Introduction (Episodes 1-3)

**Characteristics**:
- Single location
- Simple transaction
- Clear instructions
- Generous time limits

**Example**: "Pay ₱50 for street food at Maginhawa Street"

### Tier 2: Intermediate (Episodes 4-7)

**Characteristics**:
- Multiple locations
- Budget management
- Some puzzle-solving
- Moderate time pressure

**Example**: "Use ₱200 to buy 3 ingredients from different markets that start with 'M'"

### Tier 3: Advanced (Episodes 8-10)

**Characteristics**:
- Complex multi-step challenges
- Strategic decisions
- Resource optimization
- High time pressure
- Hidden information

**Example**: "Build a complete meal with ₱150, but you can only shop at merchants whose names contain letters from 'QUESTPAY'"

### Tier 4: Finals (Episode 11-12)

**Characteristics**:
- Combines all previous mechanics
- Requires all collected codes
- Mental and physical endurance
- Dramatic finale location

**Example**: "Use your earned funds to navigate a 12-hour city-wide quest culminating at a mystery final location"

---

## Contestant Tools & Resources

### QuestPay Contestant App

**Features**:
- Code scanner
- Challenge history
- Map and navigation
- Wallet balance
- Support contact
- Rules reference

### Allowed Resources

✅ Smartphone and charger  
✅ Cash for emergencies (cannot use for challenges)  
✅ Public transportation  
✅ Partner wallet app  
✅ Personal knowledge and skills  

### Prohibited Resources

❌ Outside help from non-contestants  
❌ Pre-arrangement with merchants  
❌ Using non-partner payment methods for challenges  
❌ Sharing codes with other contestants  
❌ Hacking or exploiting system vulnerabilities  

---

## Scoring System

### Base Points

| Achievement | Points |
|-------------|--------|
| Challenge completion | 100 |
| Speed bonus (top 25%) | +50 |
| Perfect execution | +25 |
| First to complete | +100 |
| Creative approach | +25 (judges' choice) |

### Penalties

| Violation | Points |
|-----------|--------|
| Rules violation | -50 |
| Late completion | -10 per minute |
| Failed attempt | -25 |
| Disqualification | All points lost |

### Special Bonuses

- **Side Quest Completion**: +10-50 points
- **Viewer Favorite**: +25 points (voted)
- **Sponsor Challenge**: +50-100 points
- **Perfect Week**: +100 points

---

## Fair Play & Integrity

### Anti-Cheating Measures

- GPS tracking of contestants
- Transaction verification against contestant ID
- Production monitors at key locations
- Whistleblower reporting system
- Post-production audit of all transactions

### Contestant Conduct

**Expected**:
- Respect for merchants and public
- Safe and legal behavior
- Honest gameplay
- Sportsmanship with fellow contestants

**Grounds for Disqualification**:
- Cheating or fraud
- Violence or harassment
- Illegal activities
- Contract violations
- Safety violations

---

[← Back to Selection](selection.md) | [Continue to Real-Time Elements →](realtime.md)
