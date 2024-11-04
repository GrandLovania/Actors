# Actors
My custom actors.

Intended for Z64Rom

Needed: (put in uLib.h)

#define ACTORFLAG_CAN_TARGET    (1)
#define ACTORFLAG_ENEMY         (1 << 2)
#define ACTORFLAG_FRIENDLY      (1 << 3)
#define ACTORFLAG_ALWAYS_UPDATE (1 << 4)

#define ACTORFLAG_ALWAYS_DRAW  (1 << 5)
#define ACTORFLAG_UNCULLED     (1 << 6)
#define ACTORFLAG_INVISIBLE    (1 << 7)
#define ACTORFLAG_TALK_REQUEST (1 << 8)

#define ACTORFLAG_HOOKSHOT_PULL   (1 << 9)
#define ACTORFLAG_HOOKSHOT_LAUNCH (1 << 10)
#define ACTORFLAG_ENKUSA_CUT      (1 << 11)
#define ACTORFLAG_NO_QUAKE        (1 << 12)

#define ACTORFLAG_HOOKSHOT_ATTACHED (1 << 13)
#define ACTORFLAG_ARROW_CAN_CARRY   (1 << 14)
#define ACTORFLAG_ARROW_ATTACHED    (1 << 15)
#define ACTORFLAG_FORCE_TALK        (1 << 16)

#define ACTORFLAG_HEAVY_OBJECT (1 << 17)
#define ACTORFLAG_CHECKSPOT    (1 << 18)
#define ACTORFLAG_SFX_AT_POS   (1 << 19)
#define ACTORFLAG_SFX_CENTER_2 (1 << 20)

#define ACTORFLAG_SFX_CENTER    (1 << 21)
#define ACTORFLAG_NO_POINTLIGHT (1 << 22)
#define ACTORFLAG_ALWAYS_THROW  (1 << 23)
#define ACTORFLAG_BODY_HIT_SFX  (1 << 24)

#define ACTORFLAG_OCARINA_UPDATE (1 << 25)
#define ACTORFLAG_PRESS_SWITCH   (1 << 26)
#define ACTORFLAG_NO_TARGET_LOCK (1 << 27)
#define ACTORFLAG_SFX_TIMER      (1 << 28)

#define new(type)    ZeldaArena_MallocDebug(sizeof(type), __FILE__, __LINE__)
#define delete(type) ZeldaArena_FreeDebug(type, __FILE__, __LINE__)

#define NEW_MATRIX() Matrix_NewMtx(__gfxCtx, __FILE__, __LINE__)
