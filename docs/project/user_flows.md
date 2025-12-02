## 1. **User Registration Flow**
**Goal: Create a new private account**
- User opens the app.
- User clicks **“Sign Up”**.
- User enters:
    - Email
    - Password
- System validates fields.

- If errors → show feedback (e.g., “Email already exists”).

- If valid → system creates user in database (Supabase Auth).

- User is automatically logged in and redirected to **Dashboard**.
    

---

## 2. **Login Flow**

**Goal: Access private workspace**

- User opens app.
    
- User clicks **“Login”**.
    
- User enters email and password.
    
- System validates credentials.
    
- If incorrect → show error.
    
- If correct → user enters **Dashboard** with private records.
    

---

## 3. **Create Record Flow**

**Goal: Add a new fossil/species record**

- User clicks **“New Record”**.
    
- User enters:
    
    - Title
        
    - Species
        
    - Description / notes
        
- Optional: user uploads images (goes to image flow).
    
- User clicks **Save**.
    
- System validates fields.
    
- System saves record to database, linked to user ID.
    
- User is redirected to:
    
    - Record detail page, **or**
        
    - Records list (depending on design).
        
- User sees confirmation.
    

---

## 4. **Add Images to a Record Flow**

**Goal: Attach visual content to a record**

- User is on **Create Record** or **Edit Record** page.
    
- User clicks **“Add Image”**.
    
- User selects file(s): JPG, PNG, WEBP.
    
- System validates size/type.
    
- Images are uploaded to **Supabase Storage**.
    
- System stores image URLs in the record’s database row.
    
- Thumbnails appear on screen.
    

**When saving the record:**

- Record data + image references are stored.
    

**If user deletes an image:**

- System removes it from storage and DB.
    

---

## 5. **Search & Filter Records Flow**

**Goal: Find specific records quickly**

- User goes to **My Records**.
    
- User types a search keyword OR applies filters:
    
    - Species
        
    - Creation date
        
    - Tags (if future feature)
        
- System queries database only for the user’s records.
    
- Results update in real time.
    
- If no matches → show **“No results found”**.
    
- User clicks a result to open it.
    

---

## 6. **Compare Information from Web Pages Flow**

**Goal: Retrieve and compare data from external sources**

- User opens a species record or a new comparison tool.
    
- User enters:
    
    - Species name
        
    - Or selects a predefined source
        
- System fetches information from multiple external sites/APIs.
    
- System normalizes and displays:
    
    - Key facts
        
    - Differences
        
    - Similarities
        
- User can:
    
    - Save selected info into a record
        
    - Copy text
        
    - Trigger AI summary (optional)
        
- If an external site fails → show a warning but continue.
    

---

## 7. **AI Assistant Query Flow**

**Goal: Ask questions about species using AI**

- User opens **AI Assistant**.
    
- User types a question (e.g., “What era did this species live in?”).
    
- System sends query to AI.
    
- AI responds with:
    
    - Explanation
        
    - Summary
        
    - Optional related suggestions
        
- User can:
    
    - Copy response
        
    - Save it into a specific record
        
    - Ask follow-up questions
        
- System logs the query to improve context for future interactions.
    

---

## 8. **Edit Record Flow**

**Goal: Modify an existing fossil record**

- User opens a record.
    
- User clicks **“Edit”**.
    
- User updates:
    
    - Text fields
        
    - Species info
        
    - Images (add/remove)
        
- User clicks **Save changes**.
    
- System validates updated data.
    
- System writes changes to database.
    
- User sees confirmation.
    

---

## 9. **Delete Record Flow**

**Goal: Permanently remove a record**

- User opens the record.
    
- User clicks **“Delete Record”**.
    
- System shows a confirmation prompt.
    
- User confirms.
    
- System deletes:
    
    - Record
        
    - Linked images
        
    - Any supplemental metadata
        
- User is redirected to **My Records** with confirmation.
